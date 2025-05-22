<!DOCTYPE html>
<html lang="es">
    <head>
        <meta charset="UTF-8">
        <title>Dashboard con Bootsstrap</title> <!--estilos ya creados, hojas de estilos que contiene todo lo que es un formato para aplicar a mi pagina web-->
        <!--<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css"
              rel="stylesheet"--> 
        <style>
            body{
                font-family: Arial, Helvetica, sans-serif;
                background-color: rgb(251, 236, 173);
                margin: 0;
                padding: 20px;
                display: flex;/*organiza el contenido en formato de caja flexible (horizontal)*/
            }
            *{
                box-sizing: border-box;/*border y padding no aumentsran su tamaño*/
            }
            /*estilos para el menu lateral*/
            .sidebar{
                width: 220px;/*ancho del menu*/
                background-color: brown;
                color: black;
                height: 100vh;/*altura completa de la ventana*/
                padding: 20px;
                position: fixed;/*mantiene fijo en su lugar al hacer scrol*/
            }
            .sidebar h2{
                margin-top: 0;/*elimina el margen superior*/
                text-align: center;
            }
            .sidebar ul{
                list-style-type: none;/*elimine los puntos de la lista*/
                padding: 0;
            }
            .sidebar li{
                padding: 10px 0;
                border-bottom: 1px solid rgba(255,255,0.2);/*linea transparente divisor*/
            }
            .sidebar ul li:hover{
                background-color: aqua;
                cursor: pointer;/*cambiar el cursor a mano*/
            }
            /*contenedor principal del contenido a la derecha*/
            .main-content{
                margin-left: 220px;/*desplazar el contenido a la derecha del menu*/
                padding: 20px;
                width:100%;/*ocupa el espacio de ancho disponible*/
            }
            h1{
                text-align: center;
                color: rgb(30, 15, 2);
            }
            .dashboard{
                display: grid;/*permite organizar los cards*/
                grid-template-columns: repeat(auto-fit,
                minmax(250px,1fr));/*ajustar columna como monimo.250 px*/
                gap: 20px;/*espacio entre trjetas*/
                margin:30px;/*espacio superior al titulo*/
            }
            .card{
                background-color:rgb(245, 210, 148);/*fondo blanco de las tarjetitas*/
                border-radius: 10px;/*bordes redondeados*/
                padding: 20px;
                box-shadow: 0 4px 8px rgb(73,38,38);/*efecto sombra*/
                text-align: center;
            }
            .card h2{
                margin: 10px 0;/*margen de arriba y abajo*/
                color: rgb(183, 36, 36);
            }
            .card p{
                font-size: 18px;
                color: chocolate;
            }
        </style>
        <body>
            <div class="sidebar">
                <h2>Menú Opciones</h2>
                <ul>
                    <li>Inicio</li>
                    <li>Resumen</li>
                    <li>Prestamos</li>
                    <li>Salir</li>
                </ul>
            </div>
            <!--contenido principal-->
            <div class="main-content">
            <h1>Dashboard Financiero-prestamos Bancario</h1>
            <div><!--viene isendo un contenedor general del dashboard-->
                <div class="dashboard">
                    <div class="card"><!--subtitulo de las tarjetas-->
                        <h2>Cuota Inicial</h2>
                        <p>S/.32,90</p>
                    </div>
                    <div class="card">
                        <h2>Monto Financiado</h2>
                        <p>S/. 122.450</p>
                    </div>
                    <div class="card">
                        <h2>Cuota Mensual</h2>
                        <p>S/.3,302.47</p>
                    </div>
            </div>
            </div>
        </body>      
    </head>
</html>
