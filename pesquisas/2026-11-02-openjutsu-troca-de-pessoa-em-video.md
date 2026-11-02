---
titulo: Openjutsu — troca de pessoa em vídeo com ComfyUI
data: 2026-11-02
tags: ia, video, comfyui, face-swap, deepfake
status: em andamento
---

# Openjutsu — troca de pessoa em vídeo com ComfyUI

## Pergunta / objetivo

Entender a ferramenta divulgada no reel de @fabianocarvalhojr: o que é, se é
mesmo local e gratuita, e o que é preciso para usar.

## Resumo

O Openjutsu é um app da Comfy-Org que troca a pessoa de um vídeo pelo
personagem de uma imagem, mantendo cena, movimento e áudio. Ao contrário do
que diz o reel, **a geração não é local nem gratuita**: só a interface roda no
seu PC, e o processamento acontece em uma GPU na nuvem da Comfy, com
cobrança. Para trocar rosto 100% local existem alternativas como o
FaceFusion para ComfyUI.

## Pontos principais

- **Como funciona:** você envia um clipe e uma imagem do personagem, escolhe
  um trecho de 5 a 15 s e recebe o trecho com a troca ([wiki](https://github.com/Comfy-Org/comfy-openjutsu/wiki)).
- **Local x nuvem:** a interface roda em `localhost:3000` (`npm run dev`), mas
  a geração usa um deployment no Comfy Developer Platform ([wiki](https://github.com/Comfy-Org/comfy-openjutsu/wiki)).
- **Custo:** consome créditos e há cobrança de GPU enquanto o deployment
  estiver ativo ([wiki](https://github.com/Comfy-Org/comfy-openjutsu/wiki)).
- **Requisitos:** Node.js 22.6+, conta e API key no Comfy Developer Platform,
  Comfy CLI. Testado em GPU de 96 GB (RTX PRO 6000).
- **Limites:** MP4/MOV de até 100 MB; plano contínuo sem cortes; o trecho
  deve começar com uma pessoa no quadro; com várias pessoas, troca a maior.
- **Modelos:** workflow H3 Character Swap (Akatz Labs), MiniMax H3, SAM 3.1 e
  GPT Image 2.5 (opcional, para a primeira imagem).
- **Licença:** app em MIT; patch do node pack em GPL-3.0; modelos com
  licenças próprias.
- **Alternativa local:** [FaceFusion ComfyUI](https://github.com/huygiatrng/Facefusion_comfyui)
  roda com inferência ONNX local e tem nó de troca em vídeo.

## Conclusões / opinião

- O reel exagera: "local e gratuito" não bate com a documentação oficial.
- O "comente o código para receber o link" é tática de engajamento; o
  repositório é público e pode ser acessado direto.
- Uso responsável: só usar com imagem de pessoas que autorizaram. No Brasil,
  uso não autorizado de imagem pode violar direito de imagem (Código Civil,
  art. 20) e, em deepfakes eleitorais ou de cunho sexual, há regras e crimes
  específicos. *(Verificar a legislação atual antes de publicar algo.)*
- Dúvida em aberto: o vídeo do reel em si não foi assistido; só a legenda foi
  lida.

## Fontes

1. [Reel de @fabianocarvalhojr no Instagram](https://www.instagram.com/reel/DfNppuykm7W/) — acessado em 2026-11-02 (somente a legenda)
2. [Comfy-Org/comfy-openjutsu — Wiki](https://github.com/Comfy-Org/comfy-openjutsu/wiki) — acessado em 2026-11-02
3. [huygiatrng/Facefusion_comfyui](https://github.com/huygiatrng/Facefusion_comfyui) — acessado em 2026-11-02

## Material original

https://www.instagram.com/reel/DfNppuykm7W/?dlrf=MTU3eDE2bm9pNTB4eQ==

## Histórico

- 2026-11-02 — criada
