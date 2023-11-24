La clase ForkJoinTask<V> es una clase abstracta cuyos metodos son usados tanto en la clase RecursiveTask que la extiende como en la clase ForkJoinPool que llama a sus metodos. 

Los metodos principales son fork(), invoke(), adapt(), join() los cuales se usan en las clases antes mencionadas.

Fork(): Divide la tarea en subtareas y las ejecuta en paralelo.Esto permite que las tareas ForkJoinTask sean muy eficientes para tareas que pueden dividirse en subtareas más pequeñas.

Invoke(): Ejecuta la tarea de manera secuencial.Esto es útil para tareas que no se pueden dividir en subtareas más pequeñas, o para tareas que se ejecutan mejor secuencialmente.

Adapt(): Convierte una tarea en otra tarea ForkJoinTask compatible. Esto es útil para tareas que no son tareas ForkJoinTask, pero que se pueden ejecutar en un ForkJoinPool.

Join(): Espera a que la tarea se complete. Esto se usa para obtener el resultado de una tarea ForkJoinTask.
