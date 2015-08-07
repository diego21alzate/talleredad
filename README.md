
<html>
    <head>
        <meta charset="UTF-8">
        <title>app discoteka</title>
    </head>
    <body>
        <form
            <form action="procesoentrar.php" method="post">
                <input required type="number" id="edad" name="edad" placeholder="digite edad" required>
                <button type="submit">enviar</button>
                
                
        </form>
            
            
    </body>
</html>

<?php
$numEdad = filter_input(INPUT_POST,"edad");


switch ($numEdad){
    
    
    case ($numEdad>=18);
        include "generos.php";
    break;

    default : include './index.php';
        break;
    
        
}

switch (true){
    case($numEdad>=18 and $numEdad<=21);
        include 'chikitka.php';
        break;
    case ($numEdad >=21 and $numEdad <40);
        include 'discotka.php';
        break;
    case ($numEdad >=40);
        include 'viejoteka.php';
        break;
   
}


<html
<head>
        <meta charset="UTF-8">
        <title>Genero</title> 
    </head>
    <body
    <form action="procesogenero.php" method="post">
     <input required type="text" id="genero" name="genero" placeholder="digite genero" required>
   
     <br>
     
  
         
     <button type="submit">enviar</button>
     
            
            <br>

        </form>
</body>
</html>
  
  
  <?php
$Genero1 = filter_input(INPUT_POST,"masculino");
$Genero2 = filter_input(INPUT_POST,"femenino");



switch (TRUE){
    case ($Genero1 === 'masculino');
        include 'vestuariohombres.php';
        break;
    
    case ($Genero2 === 'femenino');
        include 'vestuariomujeres.php';
        break;
    
    default:   include './index.php';
        break;
}


<html>
    <head>
        <meta charset="UTF-8">
        <title></title>
    </head>
    <body>
        <form action="procesovestir.php" method="post">
            <label for="camisa">Camisa</label>
            <input for="text" id="camisa" name="camisa"required>
            <br>
            
            <label for="informal">informal</label>
            <input for="text" id="informal" name="informal"required>
            <br>
            <label for="pantalon">pantalon</label>
            <input for="text" id="pantalon" name="pantalon"required>
            <br>
            <label for="zapatos">zapatos</label>
            <input for="text" id="zapatos" name="zapatos"required>
            <br>
            
            
            
     
            
            <button type="submit">enviar</button>
            
    </body>
</html>


<html>
    <head>
        <meta charset="UTF-8">
        <title> vestuario</title>
    </head>
    <body>
        <form action="procesovestir.php" method="post">
            <label for="blusa">Blusa</label>
            <input for="text" id="blusa" name="blusa" required>
            <br>
            <label for="vestido">Vestido</label>
            <input for="text" id="vestido" name="blusa" required>
            <br>
            <label for="falda">Falda</label>
            <input for="text" id="falda" name="falda" required>
            <br>
            <label for="calzado">Calzado</label>
            <input for="text" id="calzado" name="calzado" required>
            
                
            
            
            
            
        </form>
    </body>
</html>



<?php

$camisa  = filter_input(INPUT_POST,"camisa");
$informal  = filter_input(INPUT_POST,"informal");
$pantalon  = filter_input(INPUT_POST,"pantalon");
$zapatos  = filter_input(INPUT_POST,"zapatos");
$blusa = filter_input(INPUT_POST,"blusa");
$vestido = filter_input(INPUT_POST,"vestido");
$falda = filter_input(INPUT_POST,"falda");
$calzado = filter_input(INPUT_POST,"calzado");



switch ($camisa){
    
    
    case ($camisa);
        include "bienvenido.php";
break;}


switch ($informal){ 
    case ($informal); 
        echo "no dentra dejenerado";
        include "./index.php";
    break;
    }
    switch ($pantalon){
    case ($pantalon);
        include "bienvenido.php";
    break;
    }
    
    switch ($zapatos){
    case ($zapatos);
        include "bienvenido.php";
    break;

 
    default : include './index.php';
        break;

}


