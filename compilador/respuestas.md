# Compilador
Ejercicios:

En un archivo de texto `respuestas.md`:

1. Escriban qué esperan de cada uno de los pasos
a-Pre-procesador(`make preprocessing`), que se genere un archivo .pp_c
b-Compilacion I (`make assembler`), que se genere un archivo .asm que tiene las instrucciones en un lenguaje binario 
c-Compilacion II (`make object`), que se genere un archivo .o que ahora es un objeto binario
d-Linkeo (`make executable`), que se haga el linkeo entre el objeto y las librerias (o entre varios objetos si hubiera) y que se genere un .e (.exe) que es el ejecutable.


2. ¿Qué agregó el preprocesador?
Agrega muchas líneas y muchos comentarios antes de lo que tenía el otro archivo.

3. Identificar en la rutina de assembler las funciones
 las funciones identificadas son:main, printf y add numbers 

4. Explicar qué quieren decir los símbolos que se crean en el objeto
son los descriptores y las entradas, en minúscula los que no se ven. D, datos de lectura y escritura; R, datos de solo lectura; T, texto todo lo ejecutable (funciones que se ejcutan), U, no definido.

5. ¿En qué se diferencian los símbolos del objeto y del ejecutable?
Simbolos del objeto:
000000000000003c T add_numbers
0000000000000000 T main
                 U printf
Simbolos del ejecutable:
tiene muchos más simbolos, printf sigue siendo U pero ahora tiene el link de donde buscar la fuinción, los otros dos siguen siendo iguales.
0000000000400569 T add_numbers
0000000000601040 B __bss_start
0000000000601040 b completed.6973
0000000000601030 D __data_start
0000000000601030 W data_start
0000000000400470 t deregister_tm_clones
00000000004004e0 t __do_global_dtors_aux
0000000000600e18 t __do_global_dtors_aux_fini_array_entry
0000000000601038 D __dso_handle
0000000000600e28 d _DYNAMIC
0000000000601040 D _edata
0000000000601048 B _end
00000000004005f4 T _fini
0000000000400500 t frame_dummy
0000000000600e10 t __frame_dummy_init_array_entry
0000000000400778 r __FRAME_END__
0000000000601000 d _GLOBAL_OFFSET_TABLE_
                 w __gmon_start__
00000000004003e0 T _init
0000000000600e18 t __init_array_end
0000000000600e10 t __init_array_start
0000000000400600 R _IO_stdin_used
                 w _ITM_deregisterTMCloneTable
                 w _ITM_registerTMCloneTable
0000000000600e20 d __JCR_END__
0000000000600e20 d __JCR_LIST__
                 w _Jv_RegisterClasses
00000000004005f0 T __libc_csu_fini
0000000000400580 T __libc_csu_init
                 U __libc_start_main@@GLIBC_2.2.5
000000000040052d T main
                 U printf@@GLIBC_2.2.5
00000000004004a0 t register_tm_clones
0000000000400440 T _start
0000000000601040 D __TMC_END__




