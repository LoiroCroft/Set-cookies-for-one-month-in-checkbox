# Set-cookies-for-one-month-in-checkbox

<p>
	<strong>TESTE</strong>
</p>

<div id="checks">
	<input id="CB1" type="checkbox" value="ON">&nbsp;&nbsp;<label for="CB1">&nbsp;</label>Colar aqui<br>
	<input id="CB2" type="checkbox" value="ON">&nbsp;&nbsp;<label for="CB2">&nbsp;</label>Colar aqui<br>
	<input id="CB3" type="checkbox" value="ON">&nbsp;&nbsp;<label for="CB3">&nbsp;</label>Colar aqui<br>
	<input id="CB4" type="checkbox" value="ON">&nbsp;&nbsp;<label for="CB4">&nbsp;</label>Colar aqui<br>
	<input id="CB5" type="checkbox" value="ON">&nbsp;&nbsp;<label for="CB5">&nbsp;</label>Colar aqui<br>
	<input id="CB6" type="checkbox" value="ON">&nbsp;&nbsp;<label for="CB6">&nbsp;</label>Colar aqui<br>
	<input id="CB7" type="checkbox" value="ON">&nbsp;&nbsp;<label for="CB7">&nbsp;</label>Colar aqui<br>
	<input id="CB8" type="checkbox" value="ON">&nbsp;&nbsp;<label for="CB8">&nbsp;</label>Colar aqui<br>
	<input id="CB9" type="checkbox" value="ON">&nbsp;&nbsp;<label for="CB9">&nbsp;</label>Colar aqui<br>
	<input id="CB10" type="checkbox" value="ON">&nbsp;&nbsp;<label for="CB10">&nbsp;</label>Colar aqui<br>
	<input id="CB11" type="checkbox" value="ON">&nbsp;&nbsp;<label for="CB11">&nbsp;</label>Colar aqui<br>
	<input id="CB12" type="checkbox" value="ON">&nbsp;&nbsp;<label for="CB12">&nbsp;</label>Colar aqui<br>
	<input id="CB13" type="checkbox" value="ON">&nbsp;&nbsp;<label for="CB13">&nbsp;</label>Colar aqui<br>
	<input id="CB14" type="checkbox" value="ON">&nbsp;&nbsp;<label for="CB14">&nbsp;</label>Colar aqui<br>
	<input id="CB15" type="checkbox" value="ON">&nbsp;&nbsp;<label for="CB15">&nbsp;</label>Colar aqui<br>
	<input id="CB16" type="checkbox" value="ON">&nbsp;&nbsp;<label for="CB16">&nbsp;</label>Colar aqui<br>
	<input id="CB17" type="checkbox" value="ON">&nbsp;&nbsp;<label for="CB17">&nbsp;</label>Colar aqui<br>
	<input id="CB18" type="checkbox" value="ON">&nbsp;&nbsp;<label for="CB18">&nbsp;</label>Colar aqui<br>
	<input id="CB19" type="checkbox" value="ON">&nbsp;&nbsp;<label for="CB19">&nbsp;</label>Colar aqui<br>
	<input id="CB20" type="checkbox" value="ON">&nbsp;&nbsp;<label for="CB20">&nbsp;</label>Colar aqui<br>
	<input id="CB21" type="checkbox" value="ON">&nbsp;&nbsp;<label for="CB21">&nbsp;</label>Colar aqui<br>
	<input id="CB22" type="checkbox" value="ON">&nbsp;&nbsp;<label for="CB22">&nbsp;</label>Colar aqui<br>
	<input id="CB23" type="checkbox" value="ON">&nbsp;&nbsp;<label for="CB23">&nbsp;</label>Colar aqui
	<p>
		&nbsp;
	</p>
	<strong>TESTE</strong><br>
	<input id="CB24" type="checkbox" value="ON">&nbsp;&nbsp;<label for="CB24">&nbsp;</label>Colar aqui<br>
	<input id="CB25" type="checkbox" value="ON">&nbsp;&nbsp;<label for="CB25">&nbsp;</label>Colar aqui
	<script type="text/javascript">
var dcSplit, posnEq, firstGrp, lastGrp, posnCB, regEx, i=0;
 dcSplit=document.cookie.split("; ");
 regEx=(/CB\d+/);           
 for(i=0; i<dcSplit.length; i++)
  { posnEq = dcSplit[i].indexOf("=")+1;      
    posnCB=dcSplit[i].search(regEx);
    if(posnCB != -1)
      { firstGrp = dcSplit[i].substring(posnCB, posnEq-1);
        lastGrp = dcSplit[i].substring( posnEq, dcSplit[i].length);  
        document.getElementById(firstGrp).checked=eval(lastGrp);        
    }  }     
// ------
 var now=new Date(), tomorrow, allInputs, cookieStr;
 tomorrow=new Date((now.setDate(now.getDate())+(1*24*60*60*1000))).toGMTString(); 
 allInputs=document.getElementById("checks").getElementsByTagName("input");
 for(i=0; i<allInputs.length; i++){ allInputs[i].onclick=writeCookie; }
// --------   
 function writeCookie()
   { cookieStr=this.id+"="+this.checked+"; expires="+1000+"; path=/";       
     document.cookie=cookieStr;
   } 
 // -------     
</script>

	<style type="text/css">
		input {
			display: none;
		}
		input + label:before
		{
			content: '';
			display: inline-block;
			width: 1.2em;
			height: 1.2em;
			border-radius: 5px;
			margin-right: 3px;
			margin-bottom: -8px;
			border: 1.8px solid black;
			box-shadow: inset 1px 1px 3px #000000;
		}
		input:checked + label
		{
			color: #0059c7;
		}
		input:checked + label:before
		{
			background: #0059c7;
		}
	</style>

</div>

<p>
	&nbsp;
</p>
