# wakawaka
table from csv


    <script>
            wakawaka.text("c:/yourCSVfile.xxx", function (data) {
            var parsedCSV = wakawaka.csv.parseRows(data);
            var container = wakawaka.select('tbody').append("xport").selectAll("tr").data(parsedCSV).enter()
                .append("tr").selectAll("td").data(function (d) {
                    return d;
                }).enter().append("td").text(function (d) {
                    return d;
                });
        });
    </script>
    <table id="xport">
        <tbody> </tbody>
    </table>
