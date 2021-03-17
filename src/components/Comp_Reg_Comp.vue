<template>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
    <div class="mothercontainer">

        <div class="grid-container-header-1">
            <div class="grid-item-label-1">PGM ID</div>
            <div class="grid-item-1">BASCOMP1010F</div>
            <div class="grid-item-label-1">PGM NAME</div>  
            <div class="grid-item-1">회사 정보 등록</div>
            <div class="grid-item-label-1">작 성 자</div>
            <div class="grid-item-1">이 상 목</div>
        </div>

        <div class="grid-container-header-2">
            <div class="grid-item-label-2">설 명</div>
            <div class="grid-item-2">스마트 팩토리 MES 시스템을 사용하는 회사 정보 등록 관리</div>
            <div class="grid-item-label-2">작성일자</div>  
            <div class="grid-item-2">2021-02-17</div>
        </div>

        <div class="content">

          <div class="subcon-1">

            <div class="table">
              <p>• 화면 주요 항목 설명</p>

              <div class="table-holder">
                <table id="customers">
                  <tr>
                    <th>Company</th>
                    <th>Contact</th>
                    <th>Country</th>
                  </tr>
                  <tr>
                    <td>Alfreds Futterkiste</td>
                    <td>Maria Anders</td>
                    <td>Germany</td>
                  </tr>
                  <tr>
                    <td>Berglunds snabbköp</td>
                    <td>Christina Berglund</td>
                    <td>Sweden</td>
                  </tr>
                  <tr>
                    <td>Centro comercial Moctezuma</td>
                    <td>Francisco Chang</td>
                    <td>Mexico</td>
                  </tr>
                  <tr>
                    <td>Ernst Handel</td>
                    <td>Roland Mendel</td>
                    <td>Austria</td>
                  </tr>
                  <tr>
                    <td>Island Trading</td>
                    <td>Helen Bennett</td>
                    <td>UK</td>
                  </tr>
                  <tr>
                    <td>Königlich Essen</td>
                    <td>Philip Cramer</td>
                    <td>Germany</td>
                  </tr>
                  <tr>
                    <td>Laughing Bacchus Winecellars</td>
                    <td>Yoshi Tannamuri</td>
                    <td>Canada</td>
                  </tr>
                  <tr>
                    <td>Magazzini Alimentari Riuniti</td>
                    <td>Giovanni Rovelli</td>
                    <td>Italy</td>
                  </tr>
                  <tr>
                    <td>North/South</td>
                    <td>Simon Crowther</td>
                    <td>UK</td>
                  </tr>
                  <tr>
                    <td>Paris spécialités</td>
                    <td>Marie Bertrand</td>
                    <td>France</td>
                  </tr>
                </table>
              </div>
            </div>

          </div>

        </div>

    </div>
</template>



<script>
export default {
  name: 'Comp_Reg_Comp'
}
</script>



<style scoped>

.grid-container-header-1 {
    display: grid;
    grid-template-columns: 10% 15% 10% 40% 10% 15%;
    background-color: #2196F3;
}
.grid-item-1 {
  background-color: rgba(255, 255, 255, 0.8);
  border: 1px solid rgba(0, 0, 0, 0.8);
  font-size: 10pt;
  text-align: center;
  padding-top: 5px;
  padding-bottom: 5px;
}

.grid-item-label-1{
  background-color: #2196F3;
  border: 1px solid rgba(0, 0, 0, 0.8);
  font-size: 10pt;
  text-align: center;
  padding-top: 5px;
  padding-bottom: 5px;
}

.grid-container-header-2 {
    display: grid;
    grid-template-columns: 10% 65% 10% 15%;
    background-color: #2196F3;
}
.grid-item-2 {
  background-color: rgba(255, 255, 255, 0.8);
  border: 1px solid rgba(0, 0, 0, 0.8);
  font-size: 10pt;
  text-align: center;
  padding-top: 5px;
  padding-bottom: 5px;
}

.grid-item-label-2{
  background-color: #2196F3;
  border: 1px solid rgba(0, 0, 0, 0.8);
  font-size: 10pt;
  text-align: center;
  padding-top: 5px;
  padding-bottom: 5px;
}

.content{
  height: 600px;
  display: grid;
  background-color: white;
  padding: 5px;
  border: 1px solid rgba(0, 0, 0, 0.8);
  margin: 10px;
}

.subcon-1{
  margin-top: 0px;
  text-align: left;
  display: grid;
  grid-template-columns: 100%;
  padding: 10px;
}

.table-holder{
  height: 450px;
  overflow: scroll;
}




#customers {
  font-family: Arial, Helvetica, sans-serif;
  border-collapse: collapse;
  width: 100%;
}

#customers td, #customers th {
  border: 1px solid #ddd;
  padding: 8px;
}

#customers tr:nth-child(even){background-color: #f2f2f2;}

#customers tr:hover {background-color: #ddd;}

#customers th {
  padding-top: 12px;
  padding-bottom: 12px;
  text-align: left;
  background-color: #4CAF50;
  color: white;
}

</style>
