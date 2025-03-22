# magisterCiecniaDatosPuc

# Comando para crear carpetas del 1 al 8 por semana
for i in {1..10}
do
    carpeta="Bimestre$i"
    if [ ! -d "$carpeta" ]; then
        mkdir "$carpeta"
        touch "$carpeta/.gitkeep"
        echo "Carpeta creada: $carpeta (con .gitkeep)"
    else
        echo "Ya existe: $carpeta"
    fi
done


for i in {1..8}
do
    carpeta="semana$i"
    if [ ! -d "$carpeta" ]; then
        mkdir "$carpeta"
        touch "$carpeta/.gitkeep"
        echo "Carpeta creada: $carpeta (con .gitkeep)"
    else
        echo "Ya existe: $carpeta"
    fi
done