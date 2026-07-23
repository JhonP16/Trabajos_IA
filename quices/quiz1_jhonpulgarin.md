## Instrucciones

1.  Ingresen a **https://huggingface.co/spaces**.
2.  Exploren diferentes Spaces.
3.  Seleccionen uno que les parezca interesante.
4.  Interactúen con el sistema durante algunos minutos.
5.  Completen la siguiente ficha de análisis.

------------------------------------------------------------------------

# Ficha de análisis

## 1. Nombre del Space

**Nombre:** LocateAnything


**Enlace:** https://huggingface.co/spaces/nvidia/LocateAnything

------------------------------------------------------------------------

## 2. ¿Qué hace el agente?

Este agente permite montar una imagen o vídeo para detectar efectivamente los elementos que están allí dispuestos en el archivo montado, consultando mediante la barra de búsqueda el elemento que queremos detectar o inferir mediante el modelo.

------------------------------------------------------------------------

## 3. Análisis PEAS

  Elemento          Respuesta
  ----------------- ----------------------------------------------------
  **Performance**   Precisión, Detección correcta, Tiempo de respuesta, Cobertura
  **Environment**   Elementos o entorno que están en la imagen
  **Actuators**     Métricas y reportes, Asignación de etiquetas.
  **Sensors**       Imágenes y vídeos capturadas o subidas, elementos textuales

------------------------------------------------------------------------

## 4. Clasificación del entorno

Complete la siguiente tabla y justifique brevemente cada respuesta.

  Propiedad      Clasificación     Justificación
  -------------- ----------------- ---------------
  Observable     Total             Porque recibe la imagen completa y el texto de la consulta, toda la información para responder está en                                    la entrada.

  
  Determinista   Sí                Porque al pasarle la misma imagen con la misma consulta exactas, normalmente va a producir la misma                                       salida.       

  
  Episódico      Sí                Cada consulta sobre una imagen es independiente de las anteriores, no tienen que ver.    

  
  Estático       Sí                Porque el modelo no cambia la imagen o la consulta mientras la está procesando.   

  
  Discreto       No                Porque las imagenes tienen parámetros que pueden tomar una gran cantidad de valores (como los pixeles).

  
  Conocido       Sí                El modelo sabe procesar e interpretar las imagenes por su entrenamiento.           

------------------------------------------------------------------------

## 5. ¿Qué tipo de programa de agente creen que es?

Agente basado en Objetivos


Creo que es un agente basado en objetivos ya que este no solo recibe la acción inicial o un estímulo, sino que también tiene un objetivo que debe cumplir y ese objetivo guía al modelo en sus decisiones. No responde siempre de la misma manera con la misma imagen, porque por ejemplo si yo le paso otro objetivo a encontrar, me cambiará la respuesta.
Por Ejemplo, le paso una imagen con árboles y bicicletas. Si le pido que encuentre bicicletas, me dará una respuesta, si le pido árboles, me dará otra distinta.
------------------------------------------------------------------------

# Discusión en clase

Después de las presentaciones, discutiremos preguntas como:

-   ¿Dos Spaces diferentes pueden compartir el mismo tipo de entorno?
-   ¿Es posible saber con certeza qué tipo de agente implementa un Space
    únicamente observándolo?
-   ¿Qué diferencia existe entre el comportamiento observable de un
    agente y su implementación interna?

------------------------------------------------------------------------

# Reto adicional

Encuentre un Space que pueda clasificarse como:

1.  **Totalmente observable, determinista y episódico.**

R// LocateAnything. Como ya se mostró antes, este Space cumple con estas características ya que:


  Observable     Total             Porque recibe la imagen completa y el texto de la consulta, toda la información para responder está en                                    la entrada.


  Determinista   Sí                Porque al pasarle la misma imagen con la misma consulta exactas, normalmente va a producir la misma                                       salida.

 Episódico      Sí                Cada consulta sobre una imagen es independiente de las anteriores, no tienen que ver.    

3.  **Parcialmente observable, estocástico y secuencial.**

Justifique su respuesta.

------------------------------------------------------------------------
