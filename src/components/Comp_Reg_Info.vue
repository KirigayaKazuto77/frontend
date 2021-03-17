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
            <div></div>
            <div class="misc-btn-container">
              <button class="misc-btn"><i class="fa fa-file-excel-o"></i> Export to Excel</button>
              <button class="misc-btn"><i class="fa fa-search"></i> Search</button>
              <button class="misc-btn"><i class="fa fa-refresh"></i> Reload</button>
              <button class="misc-btn"><i class="fa fa-plus"></i> Add</button>
              <button class="misc-btn"><i class="fa fa-trash"></i> Delete</button>
              <button class="misc-btn"><i class="fa fa-save"></i> Save</button>
              <button class="misc-btn"><i class="fa fa-close"></i> Cancel</button>
            </div>
          </div>

          <div class="cont-header"></div>

          <div class="subcon-2">

            <div class="table">
              <p>■  회사정보목록 ( 1 )</p>

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

            <div class="form">
              <p>■ 회사정보상세</p>

              <div class="form-style-2">
                <div class="form-style-2-heading">Provide your information</div>
                  <form action="" method="post">
                    <label for="field1"><span>Name <span class="required">*</span></span><input type="text" class="input-field" name="field1" value="" /></label>
                    <label for="field2"><span>Email <span class="required">*</span></span><input type="text" class="input-field" name="field2" value="" /></label>
                    <label><span>Telephone</span><input type="text" class="tel-number-field" name="tel_no_1" value="" maxlength="4" />-<input type="text" class="tel-number-field" name="tel_no_2" value="" maxlength="4"  />-<input type="text" class="tel-number-field" name="tel_no_3" value="" maxlength="10"  /></label>
                    <label for="field4"><span>Regarding</span><select name="field4" class="select-field">
                    <option value="General Question">General</option>
                    <option value="Advertise">Advertisement</option>
                    <option value="Partnership">Partnership</option>
                    </select></label>
                    <label for="field5"><span>Message <span class="required">*</span></span><textarea name="field5" class="textarea-field"></textarea></label>

                    <label><span> </span><input type="submit" value="Submit" /></label>
                  </form>
                </div>
            </div>

          </div>

        </div>

    </div>
</template>



<script>
export default {
  name: 'Comp_Reg_Info'
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
  display: grid;
  grid-template-columns: 55% 45%;
}

.misc-btn-container{
  height: 30px;
  display: grid;
  grid-template-columns: 20% 13.5% 13.5% 12.5% 13.5% 13.5% 13.5%;
}

.misc-btn{
  background-color: black;
  font-size: 7pt;
  color: white;
  padding: 5px;
  margin-inline: 2px;
}

.cont-header{
  margin-top: 0px;
  height: 40px;
  background-color: #85bbe7;
  font-size: 25pt;
  border: 2px solid rgba(0, 0, 0, 0.4);
}

.subcon-2{
  margin-top: 0px;
  text-align: left;
  display: grid;
  grid-template-columns: 50% 50%;
  padding: 10px;
}

.table-holder{
  width: 97.5%;
  height: 200px;
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



.form-style-2{
	max-width: 500px;
	padding: 20px 12px 10px 20px;
	font: 13px Arial, Helvetica, sans-serif;
}
.form-style-2-heading{
	font-weight: bold;
	font-style: italic;
	border-bottom: 2px solid #ddd;
	margin-bottom: 20px;
	font-size: 15px;
	padding-bottom: 3px;
}
.form-style-2 label{
	display: block;
	margin: 0px 0px 15px 0px;
}
.form-style-2 label > span{
	width: 100px;
	font-weight: bold;
	float: left;
	padding-top: 8px;
	padding-right: 5px;
}
.form-style-2 span.required{
	color:red;
}
.form-style-2 .tel-number-field{
	width: 40px;
	text-align: center;
}
.form-style-2 input.input-field, .form-style-2 .select-field{
	width: 48%;	
}
.form-style-2 input.input-field, 
.form-style-2 .tel-number-field, 
.form-style-2 .textarea-field, 
 .form-style-2 .select-field{
	box-sizing: border-box;
	-webkit-box-sizing: border-box;
	-moz-box-sizing: border-box;
	border: 1px solid #C2C2C2;
	box-shadow: 1px 1px 4px #EBEBEB;
	-moz-box-shadow: 1px 1px 4px #EBEBEB;
	-webkit-box-shadow: 1px 1px 4px #EBEBEB;
	border-radius: 3px;
	-webkit-border-radius: 3px;
	-moz-border-radius: 3px;
	padding: 7px;
	outline: none;
}
.form-style-2 .input-field:focus, 
.form-style-2 .tel-number-field:focus, 
.form-style-2 .textarea-field:focus,  
.form-style-2 .select-field:focus{
	border: 1px solid #0C0;
}
.form-style-2 .textarea-field{
	height:100px;
	width: 55%;
}
.form-style-2 input[type=submit],
.form-style-2 input[type=button]{
	border: none;
	padding: 8px 15px 8px 15px;
	background: #FF8500;
	color: #fff;
	box-shadow: 1px 1px 4px #DADADA;
	-moz-box-shadow: 1px 1px 4px #DADADA;
	-webkit-box-shadow: 1px 1px 4px #DADADA;
	border-radius: 3px;
	-webkit-border-radius: 3px;
	-moz-border-radius: 3px;
}
.form-style-2 input[type=submit]:hover,
.form-style-2 input[type=button]:hover{
	background: #EA7B00;
	color: #fff;
}

</style>
