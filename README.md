Skip to content
This repository
Search
Pull requests
Issues
Marketplace
Explore
 @shiqaOsman
 Sign out
 Watch 0
  Star 0  Fork 0 shiqaOsman/Test1
 Code  Issues 0  Pull requests 0  Projects 0  Wiki  Insights  Settings
Browse files
Create sort
 master
1 parent cb83afe commit fe4c302b1c42043a96beba2d20324c55739bec28 @shiqaOsman shiqaOsman committed a minute ago  Verified
Unified Split
Showing  1 changed file  with 104 additions and 0 deletions.
View  
104  sort
@@ -0,0 +1,104 @@
 +<!DOCTYPE html>
 +<html>
 +<head>
 +<title>Sort a HTML Table Alphabetically</title>
 +<style>
 +table {
 +    border-spacing: 0;
 +    width: 100%;
 +    border: 1px solid #ddd;
 +}
 +
 +th, td {
 +    text-align: left;
 +    padding: 16px;
 +}
 +
 +tr:nth-child(even) {
 +    background-color: #f2f2f2
 +}
 +</style>
 +</head>
 +<body>
 +
 +<p>Click the button to sort the table alphabetically, by name:</p>
 +<p><button onclick="sortTable()">Sort</button></p>
 +
 +<table id="myTable">
 +  <tr>
 +    <th>Name</th>
 +    <th>Country</th>
 +  </tr>
 +  <tr>
 +    <td>Berglunds snabbkop</td>
 +    <td>Sweden</td>
 +  </tr>
 +  <tr>
 +    <td>North/South</td>
 +    <td>UK</td>
 +  </tr>
 +  <tr>
 +    <td>Alfreds Futterkiste</td>
 +    <td>Germany</td>
 +  </tr>
 +  <tr>
 +    <td>Koniglich Essen</td>
 +    <td>Germany</td>
 +  </tr>
 +  <tr>
 +    <td>Magazzini Alimentari Riuniti</td>
 +    <td>Italy</td>
 +  </tr>
 +  <tr>
 +    <td>Paris specialites</td>
 +    <td>France</td>
 +  </tr>
 +  <tr>
 +    <td>Island Trading</td>
 +    <td>UK</td>
 +  </tr>
 +  <tr>
 +    <td>Laughing Bacchus Winecellars</td>
 +    <td>Canada</td>
 +  </tr>
 +</table>
 +
 +<script>
 +function sortTable() {
 +  var table, rows, switching, i, x, y, shouldSwitch;
 +  table = document.getElementById("myTable");
 +  switching = true;
 +  /*Make a loop that will continue until
 +  no switching has been done:*/
 +  while (switching) {
 +    //start by saying: no switching is done:
 +    switching = false;
 +    rows = table.getElementsByTagName("TR");
 +    /*Loop through all table rows (except the
 +    first, which contains table headers):*/
 +    for (i = 1; i < (rows.length - 1); i++) {
 +      //start by saying there should be no switching:
 +      shouldSwitch = false;
 +      /*Get the two elements you want to compare,
 +      one from current row and one from the next:*/
 +      x = rows[i].getElementsByTagName("TD")[0];
 +      y = rows[i + 1].getElementsByTagName("TD")[0];
 +      //check if the two rows should switch place:
 +      if (x.innerHTML.toLowerCase() > y.innerHTML.toLowerCase()) {
 +        //if so, mark as a switch and break the loop:
 +        shouldSwitch= true;
 +        break;
 +      }
 +    }
 +    if (shouldSwitch) {
 +      /*If a switch has been marked, make the switch
 +      and mark that a switch has been done:*/
 +      rows[i].parentNode.insertBefore(rows[i + 1], rows[i]);
 +      switching = true;
 +    }
 +  }
 +}
 +</script>
 +
 +</body>
 +</html>
 Lock conversation 0 comments on commit fe4c302
@shiqaOsman
  
            
 
Write  Preview

Leave a comment
Choose Files Attach files by dragging & dropping, selecting them, or pasting from the clipboard.  Styling with Markdown is supported
Comment on this commit
   Subscribe  You’re not receiving notifications from this thread.
© 2017 GitHub, Inc.
Terms
Privacy
Security
Status
Help
Contact GitHub
API
Training
Shop
Blog
About
