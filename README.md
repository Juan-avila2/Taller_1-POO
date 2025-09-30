# Taller_1-POO

Respuestas
1. A, B y D
2. False True
3. a) Falso, ya que al colocar _ Python no impide el acceso, esto solo sirve como "metodo de acvertencia" para que otra persona no lo use, pero no hay nada que lo impida.
   b) Falso, ya que al usar __ Python "manglea" el nombre del atributo, pero aún es accesible si se conoce el nombre "mangleado"
   c) Verdadero, el mangling coloca primero el nombre de la clase, y despues el del atributo 
4. Se imprime: abc, no hay error, porque _token solo tiene un _, así que Python no hace mangling ni restringe de ninguna manera el atributo token, solo indica que es protegido.
5. Se imprime: (2,1)
6. Hay un error al tratar de ejecutar la línea c.y = 20, ya que "__slots__ = ('x',)" restringe los atributos que se pueden ingresar a x, por lo que al tratar de ingresar y, se genera el error
7. self._atributo = 99
8. Imprime: True False True, _step existe tal cual; __tick se mangla a _M__tick, por lo que hasattr(m,'__tick') es False , pero hasattr(m,'_M__tick') es True.
9. print(s._S__data)
10. El nombre más probable en la lista es _D__a, porque __a se manglea a _D__a, por lo que dir(d) mostrará _D__a. No aparecerá __a ni a porque el atributo fue renombrado internamente.
11.
<img width="747" height="356" alt="image" src="https://github.com/user-attachments/assets/0edd40f7-8ad2-4bc3-88fa-46e1ac303aa1" />
12.
<img width="565" height="178" alt="image" src="https://github.com/user-attachments/assets/2fbbdb8f-6141-4d40-bfcc-17363dc2f4a8" /> 
13. 
<img width="679" height="328" alt="image" src="https://github.com/user-attachments/assets/08eb79c6-540b-44ad-9e4d-3f810fa459bb" />
14.
<img width="780" height="270" alt="image" src="https://github.com/user-attachments/assets/a7e4a081-b0b0-4c9d-b8c1-d18e1df48152" />
15.
<img width="897" height="457" alt="image" src="https://github.com/user-attachments/assets/426ab4c0-9c55-435e-b8d4-fa1014c0fc51" />
16. Usaría _atributo para señalar uso interno y __atributo solo cuando quieras evitar colisiones en subclases mediante name mangling.
17. El rpoblema es que get_data() devuelve la referencia interna, el llamador puede modificarla y corromper el estado interno (fuga de encapsulación).
<img width="401" height="67" alt="image" src="https://github.com/user-attachments/assets/89c3afbb-0bf3-40d2-9fe8-cb48cfe3d947" />
18. Falla en que B.get() intenta acceder a __x pensando que es el mismo nombre; pero __x en A se manglea a _A__x, y __x en B esperaría _B__x.
por tanto self.__x en B no encontrará _A__x y fallará con AttributeError.
<img width="341" height="159" alt="image" src="https://github.com/user-attachments/assets/61f4cb5d-b0fc-4d31-a6d8-93b9915132d8" />
19. 
<img width="456" height="146" alt="image" src="https://github.com/user-attachments/assets/26e6104b-328c-4a96-b72a-84ed8ab60bfd" />
20. Solución en archivo
