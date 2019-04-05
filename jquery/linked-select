```
<select id="hour1"></select>
<select id="hour2"></select>

<script>
//jquery는 이미 import되어 있다는 가정하에 작성함.
$(function(){
	var hours = "";
	for(let i = 0; i < 24; i++){
		let hour = i < 10 ? "0" + i : i;
		hours += `<option value="${hour}">${hour}시</>`;
	}
	$("select").html(hours);
	
	$("select").on("change", function(e){
		let $this = $(e.target);
		let $idx = $this.index();
		if($idx === 0){ //앞에꺼
			$("select").eq(1).val(Number($this.val()) + 1);
		}else{ //뒤에거
			$("select").eq(0).val(Number($this.val()) - 1);
		}
	});
});
</script>
```
