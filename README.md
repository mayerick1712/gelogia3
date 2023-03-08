<!DOCTYPEhtml >
<html> _ _
  < cabeza >
    < juego de caracteres meta  =" UTF-8 " >
    < title > Mi ubicación GPS </ title >
  </ cabeza >
  < cuerpo >
    < h1  id =" ubicación " > Cargando ubicación... </ h1 >
    < guión >
      if  ( navegador . geolocalización )  {
        navegante _ geolocalización _ getPosiciónActual ( función ( posición )  {
          var  latitud  =  posición . coordenadas _ latitud ;
          var  longitud  =  posición . coordenadas _ longitud ;
          documento _ getElementById ( "ubicación" ) . HTML interno  =
            "Latitud: "  +  latitud  +  "<br>Longitud: "  +  longitud ;
        } ) ;
      }  más  {
        documento _ getElementById ( "ubicación" ) . HTML interno  =
          "Lo siento, tu navegador no soporta la ubicación GPS". ;
      }
    </ guión >
  </ cuerpo >
</html> _ _
