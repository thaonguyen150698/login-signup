function newStyle() {
  let newColor = '';
  let newFont = ''; 
  let x = Math.floor(Math.random()*7); 
  switch (x){
    case 0:
      newColor = 'red';
      newFont = 'Times New Roman'; 
      break;
    case 1: 
      newColor = 'pink';
      newFont = 'Florence, cursive'; 
      break;
    case 2:
      newColor = 'yellow';
      newFont = 'Verdana';
      break; 
    case 3:
      newColor= 'purple';
      newFont = 'Courier New';
      break
    case 4:
      newColor = 'cyan';
      newFont = 'Georgia'; 
      break;
    case 5:
        newColor = 'maroon';
        newFont = 'Palatino';
        break;
    case 6: 
        newColor = 'lime';
        newFont = 'Impact';
        break;
  }
  var elem = document.getElementById('logo');
  elem.style.color = newColor;
  elem.style.fontFamily = newFont; 
}
function showLocation(){
  var checkbox = document.getElementById('chk');
  var output = document.getElementsByClassName('hidden');
  for(var i = 0; i != output.length;i++){
	if(checkbox.checked){
		output[i].style.display = 'block';
		
	}else{
		output[i].style.display = 'none';
	}
  }
}