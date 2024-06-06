# EmpathicZoom

Instalar ambiente
```
conda env create -f environment.yml
```

Actualizar ambiente en caso de intalar nuevas dependencias
```
conda env export > environment.yml
```

Importante: eliminar la última fila del archivo environment.yml ("prefix: C:\Users\{user}\miniconda3\envs\empathic-zoom").