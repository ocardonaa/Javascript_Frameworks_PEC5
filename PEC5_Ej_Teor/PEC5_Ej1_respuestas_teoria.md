## a) ¿Cuáles son las principales diferencias entre formularios dirigidos por template y formularios reactivos?
- Mientras que los template forms se crean de forma declarativa, siguiendo un modelo más lógico para crear un form, los reactive se crean de forma imperativa, y la lógica está definida en el componente. Los template tienen una curva de aprendizaje más baja, pero los reactive aprovechan que solo escuchan cuando se ha lanzado un evento, por lo que serán más eficientes.

## b) ¿Qué son, para qué sirven y cómo se utilizan las directivas ngModel y ngModelChange?
- Ambas son directivas, que extraen el valor de los inputs, facilitando el crear webs. Para usarlos los escribimos dentro de un input de html de la siguiente forma:
        [ngModel]="stock.name"
        (ngModelChange)="stock.name=$event"
  Donde extrae el atributo stock.name y si se triguerea un cambio ($event), lo capta con ngModelChange y lo actualiza

## c) ¿Qué son, cuáles son y para qué sirven los estados en los formularios dirigidos por templates?
- ng-touched y ng-untouched: si se ha interactuado o no con el formulario
- ng-dirty y ng-pristine: si ha hecho cambios o no en el formulario
- ng-valid y ng-invalid: si el usuario ha introducido en el formulario un valor válido o inválido

## d) ¿Qué ventajas aportan los FormGroup en la composición de formularios?
- Sus principales ventajas, a parte de ofrecer un código más limpio, un sistema de validación, facilitar el testing, separar responsabilidades y poder integrar librerias externas es, que el formulario pasa a ser reactivo, de modo que permite forms más dinamicos y responsive además de la eficiencia de los reactive forms.