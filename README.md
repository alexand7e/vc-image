# Cyberpunk Hand Particles

Mini-projeto em **Three.js + MediaPipe Hands**: um sistema de **12.000 partículas neon** com estética cyberpunk, controlado por gestos das mãos via webcam.

## Como usar

1. Rode em um servidor local (webcam não funciona bem em `file://`).
2. Abra no navegador e permita acesso à câmera.

### Opção A (Python)

```bash
python -m http.server 5173
```

Acesse: `http://localhost:5173/`

### Opção B (Node)

```bash
npx serve .
```

## Controles (gestos)

### Mão esquerda (comando)
- 1 dedo: “Hello” (ciano neon)
- 2 dedos: “Gemini3” (amarelo neon)
- 3 dedos: “非常好用” (rosa neon)
- 4 dedos: “再见” (verde neon)
- 5 dedos: **Modo Captura** (atração para a palma esquerda)

### Mão direita (interação)
- Padrão: repulsão/“scatter” ao tocar as partículas (apenas no plano XY)
- 5 dedos: **Modo Nebulosa** (partículas ocupam o espaço 3D + ripple ao mover a mão)

### Combo (ultimate)
- Mão direita aberta (Nebulosa) + mão esquerda aberta (Captura): partículas formam uma **bola de basquete 3D** na mão esquerda.

## Estrutura

```
.
├─ index.html
├─ css/
│  └─ styles.css
└─ assets/
   ├─ manifest.webmanifest
   ├─ icon.svg
   └─ favicon.svg
```
