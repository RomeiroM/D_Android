# ✅Aula 01 - Lógica de programação

## 🎮Desafios do jogo Blockly

### 🤨O que é?

Blockly é uma ferramenta visual que tem por objetivo auxiliar na compreensão sobre a funcionalidade de uma linguagem de programação. 

Provavelmente você já ouviu falar no Scratch, que também é uma ferramenta de programação em blocos de caráter mais lúdico, sendo que o Blockly é considerado um pouco mais evoluído. Estudantes de TI costumam estudar o Scratch no início da graduação, visto que auxilia na prática de algoritmos, servindo de “trampolim” no aprendizado de outras linguagens como C e Java. [ler mais.](https://blog.cronapp.io/programacao-blockly-saiba-mais-sobre-essa-linguagem-visual/)

### Labirinto

- [Desafio 2](https://blockly.games/maze?lang=pt-br&level=2&&skin=0#3kc8sf)

<div align="center">
  <p>Trilha e código do desafio</p>
  <p float="left">
  <img src="https://github.com/RomeiroM/Kotlin/assets/85644789/4ce3ac97-95a6-4715-87c5-3195acc70225" width="200">
  <img src="https://github.com/RomeiroM/Kotlin/assets/85644789/bcd39c15-fb3f-4dcc-bc85-027bfb968e16" width="200">
  </p>
</div>

Código em JavaScript:
````JavaScript
moveForward();
turnLeft();
moveForward();
turnRight();
moveForward();
````

- [Desafio 3](https://blockly.games/maze?lang=pt-br&level=3&skin=0#ykg7bn)

<div align="center">
  <p>Trilha e código do desafio</p>
  <p float="left">
  <img src="https://github.com/RomeiroM/Kotlin/assets/85644789/30100d59-fe86-408d-8779-a379642a73f3" width="200">
  <img src="https://github.com/RomeiroM/Kotlin/assets/85644789/9da2704a-24e6-428f-a80c-15ddef3e7fc0" width="200">
  </p>
</div>

Código em JavaScript:
````JavaScript
while (notDone()) {
  moveForward();
}
````

- [Desafio 4](https://blockly.games/maze?lang=pt-br&level=4&&skin=0#3i5hsz)

<div align="center">
  <p>Trilha e código do desafio</p>
  <p float="left">
  <img src="https://github.com/RomeiroM/Kotlin/assets/85644789/ba3e8bda-c8e8-4a4a-b510-c392c36b09e9" width="200">
  <img src="https://github.com/RomeiroM/Kotlin/assets/85644789/fe99ae12-f175-4b6e-835b-739778b595c6" width="200">
  </p>
</div>

Código em JavaScript:
````JavaScript
while (notDone()) {
  moveForward();
  turnLeft();
  moveForward();
  turnRight();
}
````

- [Desafio 5](https://blockly.games/maze?lang=pt-br&level=5&skin=0#n4s8sm)

<div align="center">
  <p>Trilha e código do desafio</p>
  <p float="left">
  <img src="https://github.com/RomeiroM/Kotlin/assets/85644789/cbeb6f5d-ce8c-42c2-b678-d095b1da0c51" width="200">
  <img src="https://github.com/RomeiroM/Kotlin/assets/85644789/8db29944-88f4-49be-893f-649d92427720" width="200">
  </p>
</div>

Código em JavaScript:
````JavaScript
moveForward();
moveForward();
turnLeft();
while (notDone()) {
  moveForward();
}
````

- [Desafio 6](https://blockly.games/maze?lang=pt-br&level=6&skin=0#4ga2fn)

<div align="center">
  <p>Trilha e código do desafio</p>
  <p float="left">
  <img src="https://github.com/RomeiroM/Kotlin/assets/85644789/f2ec7798-c9a2-4feb-9b62-0a63fd221cf7" width="200">
  <img src="https://github.com/RomeiroM/Kotlin/assets/85644789/787d8787-1000-46ca-8f57-f818b888a679" width="200">
  </p>
</div>

Código em JavaScript:
````JavaScript
while (notDone()) {
  moveForward();
  if (isPathLeft()) {
    turnLeft();
  }
}
````

- [Desafio 7](https://blockly.games/maze?lang=pt-br&level=7&skin=0#csvscb)

<div align="center">
  <p>Trilha e código do desafio</p>
  <p float="left">
  <img src="https://github.com/RomeiroM/Kotlin/assets/85644789/9df39c6b-6ee0-45d6-90be-ea4a7f29c204" width="200">
  <img src="https://github.com/RomeiroM/Kotlin/assets/85644789/b5050237-34c1-46f9-928e-3dca14be6f1b" width="200">
  </p>
</div>

Código em JavaScript:
````JavaScript
while (notDone()) {
  if (isPathForward()) {
    moveForward();
  }
  if (isPathRight()) {
    turnRight();
  }
}
````

- [Desafio 8](https://blockly.games/maze?lang=pt-br&level=8&skin=0#baihzz)

<div align="center">
  <p>Trilha e código do desafio</p>
  <p float="left">
  <img src="https://github.com/RomeiroM/Kotlin/assets/85644789/07fe9507-2801-497b-aa59-c7b789557fe4" width="200">
  <img src="https://github.com/RomeiroM/Kotlin/assets/85644789/605c81ac-2530-4a9c-bf25-6ccf43e07fa3" width="200">
  </p>
</div>

Código em JavaScript:
````JavaScript
while (notDone()) {
  moveForward();
  if (isPathRight()) {
    turnRight();
  }
  if (isPathLeft()) {
    turnLeft();
  }
}
````

- [Desafio 9](https://blockly.games/maze?lang=pt-br&level=9&skin=0#jhkof3)

<div align="center">
  <p>Trilha e código do desafio</p>
  <p float="left">
  <img src="https://github.com/RomeiroM/Kotlin/assets/85644789/082eb6ec-eb0f-4a17-9df6-31d69a90e10a" width="200">
  <img src="https://github.com/RomeiroM/Kotlin/assets/85644789/53784da2-fbea-4890-9214-2f2df5edc022" width="200">
  </p>
</div>

Código em JavaScript:
````JavaScript
while (notDone()) {
  if (isPathForward()) {
    moveForward();
  } else {
    turnLeft();
  }
}
````

- [Desafio 10](https://blockly.games/maze?lang=pt-br&level=10&skin=1#8d9z2y)

<div align="center">
  <p>Trilha e código do desafio</p>
  <p float="left">
  <img src="https://github.com/RomeiroM/Kotlin/assets/85644789/c3d19f9a-518f-482a-a7ec-1ca6d400f13e" width="200">
  <img src="https://github.com/RomeiroM/Kotlin/assets/85644789/ce3b5775-eba6-4d00-a202-ad2a8b7b5e8b" width="200">
  </p>
</div>

Código em JavaScript:
````JavaScript
while (notDone()) {
  moveForward();
  if (isPathRight()) {
    if (isPathForward()) {
      turnRight();
    } else {
      if (isPathLeft()) {
        turnLeft();
      } else {
        turnRight();
      }
    }
  } else {
    if (isPathLeft()) {
      turnLeft();
    }
  }
}
````
### Pássaro

- [1](https://blockly.games/bird?lang=pt-br&level=1#xsismq)
- [2](https://blockly.games/bird?lang=pt-br&level=2#562ubo)
- [3](https://blockly.games/bird?lang=pt-br&level=3#dq8zdv)
- [4](https://blockly.games/bird?lang=pt-br&level=4#4vcqnn)
- [5](https://blockly.games/bird?lang=pt-br&level=5#ahqtvs)
- [6](https://blockly.games/bird?lang=pt-br&level=6#e9pwsj)
- [7](https://blockly.games/bird?lang=pt-br&level=7#yvmc9h)
