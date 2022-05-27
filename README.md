# Tarea-3 Part_1

# Pasos para realizar la tarea  N.3

1.Para empezar se utilizo el programa Git Bash 
2. Seguidoi se ubico en la ruta  : HP@DESKTOP-ARATL58 MINGW64 ~/documents/CSB-master/unix/data/Saavedra2013 
3. touch netsize.sh 

# seguido  se ubico el directorio y la ruta    
3.fila=`wc -l < n1.txt`
      *donde "<" hace que rl contenido de n1.txt se envie a ala funcion wc -l ya que este es el contador de filas  
      
4.column=` awk "{print NF} n1.tx  | head -n 1`
       *"head" muestra la primera linea del archivo n1.txt
       *awk "{print NF}" este proporcional el numero de columnas que hay en un registro

# finalmente  se imprime utilizando
 5.echo "El numero de filaas y columnas de n1.txt son: $fila, $columna." >> netsize.txt
 6. bash netsize.sh   
      *sirve para rrecorer 
      
      
# Tarea-3 Part_2

1.Para empezar se utilizo el programa Git Bash 
2. Seguidoi se ubico en la ruta  : HP@DESKTOP-ARATL58 MINGW64 ~/documents/CSB-master/unix/data/Saavedra2013 
3. touch netsize_all.sh 

# seguido  se ubico el directorio y la ruta      
3.for archivo in *.txt

  do
         numero_fila=`cat $archivo | wc -l`
         numero_columna=`head -n 1 $archivo | tr -d " " | tr -d "\n" | wc -c`
         echo "El numero de filaas y columnas de $archivo son: $numero_fila, $numero_columna." >> netsize_all.txt
  done

      
# finalmente  se imprime utilizando
 5. bash netsize_all.sh 
      *sirve para rrecorer 
 
 
 
 
 
