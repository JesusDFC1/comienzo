<script>
     export let pais;
     let p;
    const paises = {   
    "colombia": ["Colombia", "Bogotá", "51.52 millones", "Peso colombiano", "1,142 millones km²", "Flag_of_Colombia.svg", "Español"],
    "venezuela": ["Venezuela", "Caracas", "28.2 millones", "Bolívar", "916,445 km²", "Flag_of_Venezuela.svg", "Español"],
    "ecuador": ["Ecuador", "Quito", "17.8 millones", "Dólar estadounidense", "256,370 km²", "Flag_of_Ecuador.svg", "Español"],
    "peru": ["Perú", "Lima", "33.72 millones", "Sol peruano", "1,285,215 km²", "Flag_of_Peru.svg", "Español"],
    "brasil": ["Brasil", "Brasilia", "214.3 millones", "Real brasileño", "8,51 millones km²", "flag_of_Brazil.svg", "Portugués"],
    "argentina": ["Argentina", "Buenos Aires", "45.38 millones", "Peso argentino", "2,780 millones km²", "Flag_of_Argentina.svg", "Español"],
    "bolivia": ["Bolivia", "Sucre", "11.35 millones", "Boliviano", "1,098 millones km²", "Flag_of_Bolivia.svg", "Español"],
    "chile": ["Chile", "Santiago", "19.45 millones", "Peso chileno", "756,102 km²", "Flag_of_Chile.svg", "Español"],
    "paraguay": ["Paraguay", "Asunción", "7.15 millones", "Guaraní", "406,752 km²", "Flag_of_Paraguay.svg", "Español, Guaraní"],
    "uruguay": ["Uruguay", "Montevideo", "3.46 millones", "Peso uruguayo", "176,215 km²", "Flag_of_Uruguay.svg", "Español"],
    "surinam": ["Surinam", "Paramaribo", "0.59 millones", "Dólar surinamés", "163,820 km²", "Flag_of_Suriname.svg", "Neerlandés"],
    "ganauy": ["Guyana", "Georgetown", "0.78 millones", "Dólar guyanés", "214,969 km²", "Flag_of_Guyana.svg", "Inglés"],
    "trinidad y tobago": ["Trinidad y Tobago", "Puerto España", "1.39 millones", "Dólar de Trinidad y Tobago", "5,130 km²", "Flag_of_Trinidad_and_Tobago.svg", "Inglés"]
  
     };
  
   
   
  
   
     p = paises[pais];
  </script>
  
  <div class="main">
    <div class="col1">
      <img src="./src/assets/{p[5]}" alt="Bandera_Colombia" width="300" height="200">
    </div>
    <div class="col2">
      <div class="linea"><strong>País:</strong> {p[0]}</div>
      <div class="linea"><strong>Capital:</strong> {p[1]}</div>
      <div class="linea"><strong>Población:</strong> {p[2]}</div>
      <div class="linea"><strong>Moneda:</strong> {p[3]}</div>
      <div class="linea"><strong>Extensión:</strong> {p[4]}</div>
      <div class="linea"><strong>Idioma:</strong> {p[6]}</div>
    </div>
  </div>
  
  <style>
    .main {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      grid-gap: 5px;
      border-radius: 10px;
      border: 2px solid rgb(186, 190, 182);
      width: 600px;
      box-shadow: 5px 5px 5px black;
      margin-right: 5px;
      margin-bottom: 10px;
    }
  
    .col1 {
      margin: 5px;
      padding: 5px;
    }
  
    .col2 {
      margin: 5px;
      padding: 5px;
      border-left: 2px solid black;
    }
  
    strong {
      color: blue;
      font-weight: bolder;
    }
  
    .linea {
      font-size: 20px;
      margin-bottom: 18px;
    }
  </style>
  