/*
 Imagen creada por Harold Aguilar Mejia
 Imagen de una pelota de tenis iluminada por una lámpara
 usando una textura para representar la pelota 
*/

#include "colors.inc"
//establecemos un fondo de color gris
background {
    color Gray
}
//posicionamos la camara
camera{
    location<2,0.5,-5>
    look_at<2,0.7,0>
}
//representamos la lampara por medio del spotlight
//le decimos que tiene un radio de 5 y el falloff nos ayuda 
// a representar la iluminación de la lámpara en el piso
// de igual manera le decimos que la luz apunta hacia el point_at
light_source{
    <2,10,0>
    color White
    spotlight
    radius 5
    falloff 15
    point_at <2, 0, 0>
}
//creamos la esfera en primer instancia, asignando su localización y radio
sphere{
    <2,0.7,0>, 0.7
    //le asignamos una textura
    texture{
        pigment{
            //dado que se usara una imagen para representar el aspecto de la pelota 
            //usamos image_map, dentro primero asignamos el tiepo de archivo que es
            // que esta dentro de los permitidos por POV-Ray, depues entre comillas el nombre 
            // del archivo, solo así ya que la imagen se encuentra en la misma carpeta donde se encuentra 
            // este codigo
            image_map{
                jpeg "pt.jpeg"
            }
        }
        // se escala la imagen de la textura para poder posicionar la imagen de la manera deseada
        // para que se persiva correctamente la pelota
        scale <-1.33,1.3,1>
    }
    //le asignamos a la pelota el dipo de reflecxión que se deasea
    finish{
        diffuse 2
        ambient 0.3
    }
}
//creamos el plano, que nos servira como piso donde esta la pelota
// justo por debajo de la pelota y de color gris 
plane{
    <0,0.8,0>0
    pigment{
        color Gray
    }
}