<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<title>Carte interactive Marvel - New York</title>
<style>
  body { margin:0; background:#111; color:white; font-family:Arial, sans-serif; }
  h1 { text-align:center; margin:20px; }
  .map { 
    position:relative; 
    max-width:1000px; 
    margin:20px auto; 
    border:3px solid red; 
    border-radius:10px; 
    overflow:hidden;
  }
  .map img { 
    width:100%; 
    display:block;
  }
  .point {
    position:absolute; 
    cursor:pointer; 
    font-size:30px;
    transform:translate(-50%,-50%);
  }
  .popup {
    position:absolute; 
    background:#222; 
    padding:10px; 
    border-radius:8px;
    display:none; 
    width:220px; 
    text-align:center;
    border:1px solid #ff4444;
    z-index:10;
  }
  .popup h3 { margin:5px 0; color:#ff4444; }
  .popup p { font-size:14px; }
</style>
</head>
<body>
<h1>🗽 Carte des héros Marvel à New York</h1>
<div class="map">
  <img src="https://upload.wikimedia.org/wikipedia/commons/4/4f/New_York_City_Map.png" alt="Carte New York">

  <!-- Spider-Man (Queens) -->
  <div class="point" style="top:65%; left:80%;" 
       onclick="showPopup(event,'Spider-Man','Le héros de Queens, créé en 1962 par Stan Lee et Steve Ditko.')">🕷️</div>

  <!-- Daredevil (Hell’s Kitchen) -->
  <div class="point" style="top:45%; left:48%;" 
       onclick="showPopup(event,'Daredevil','Le justicier aveugle de Hell’s Kitchen, avocat le jour, héros la nuit.')">👓</div>

  <!-- Captain America (Brooklyn) -->
  <div class="point" style="top:75%; left:60%;" 
       onclick="showPopup(event,'Captain America','Steve Rogers est né à Brooklyn et devint le premier Avenger.')">🛡️</div>

  <!-- Avengers Tower (Manhattan) -->
  <div class="point" style="top:50%; left:55%;" 
       onclick="showPopup(event,'Avengers','QG des Avengers situé à Manhattan.')">🏢</div>

  <!-- Popup -->
  <div id="popup" class="popup"></div>
</div>

<script>
function showPopup(e,title,desc){
  const popup=document.getElementById("popup");
  popup.style.left = e.target.style.left;
  popup.style.top = e.target.style.top;
  popup.innerHTML=`<h3>${title}</h3><p>${desc}</p>`;
  popup.style.display="block";
}
</script>
</body>
</html>
