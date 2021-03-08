# basic-course-JavaScript-5
<meta charset="utf-8">
<script>
var table = document.createElement("table");
var letters = "abcdefgh";
function ChessBoard(h,w){
    for(war i = 1; i<h; i++){
        var tr = document.createElement("tr");
        for (var j = 1; j<w; j++){
            var td = document.createElement("td");
            if (i == 1 || i == 10){
                td.className = "noBorder";
                if (j >= 2 && i <9){
                    td.innerHTML = -(i - 10);
                }
            }else if (i % 2 == j % 2){
                td.className = "white";
            }else{
                td.className = "black";
            }
            if (i == 3){
                if (j>=2 && j <= 9){
                td.innerHTML = "<img src='./figures/pawnBlack.svg'>";
                }
            }else if (i == 2) {
                if (j == 2 || j == 9){
                td.innerHTML = "<img src='./figures/rookBlack.svg'>";
            }else if (j == 3 || j == 8) {
                 td.innerHTML = "<img src='./figures/rookBlack.svg'>";
            }else if (j == 4 || j == 7) {
                td.innerHTML = "<img src='./figures/elephantBlack.svg'>";
            }else if (j == 5){
                td.innerHTML = "<img src='./figures/geenBlack.svg'>";
            }else if (j == 6){
                td.innerHTML = "<img src='./figures/kingBlack.svg'>";}
            }
        }else if (i == 8) {
            if (j >=2 && j <= 9) {
                d.innerHTML = "<img src='./figures/pawnWhite.svg'>";}
            }
        }else if (i == 9) {
                if (j == 2 || j == 9){
                td.innerHTML = "<img src='./figures/rookWhite.svg'>";
            }else if (j == 3 || j == 8) {
                 td.innerHTML = "<img src='./figures/horseWhite.svg'>";
            }else if (j == 4 || j == 7) {
                td.innerHTML = "<img src='./figures/elephantWhite.svg'>";
            }else if (j == 5){
                td.innerHTML = "<img src='./figures/geenWhite.svg'>";
            }else if (j == 6){
                td.innerHTML = "<img src='./figures/kingWhite.svg'>";}
            }
         }
         tr.appenChild(td);
    }
    table.appendChild(tr);
}
document.body.appendChild(table);
}
ChessBoard(11;11);
</script>
  
