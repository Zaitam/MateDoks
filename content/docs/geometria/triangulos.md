---
title: "Triangulos"
description: ""
date: 2022-06-06T21:26:27-03:00
lastmod: 2022-06-06T21:26:27-03:00
draft: false
images: []
---

## Clasificacion

### Angulos

Acutangulo = 3 Angulos Agudos

Rectangulo = 1 Angulo recto

Obstusangulo = 1 Angulo obstuso

### Lados

Isosceles = 2 lados iguales

Escaleno = Todos los lados distintos

Equilatero = 3 lados iguales

---
<script type="text/tikz">
  \begin{tikzpicture}
    \draw (0,0)node[below left]{A} --
  ++(2,0)node[below right]{C}coordinate(C) --
  ++(0,2)node[below right]{B} -- cycle;
  \draw (C) +(-3mm,0mm) |- +(0mm,3mm);
  \end{tikzpicture}
</script>
