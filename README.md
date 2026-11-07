# nordesterp-vehicles-images
## vehicles/

Fotos dos veículos (NordesteRP S4) para a garagem/concessionária do `snt-vehicles` e as outras telas
(`snt-fuelstations`, `nrp_recompensas`, `tablet_admin`, `combo_lucky`, `combo_livestream`).

- `vehicles/<modelo>.webp` — **o que as telas usam**: WebP 512x512 com perda (qualidade 75), alfa sem perda, sem
  fundo, ~12 KB. URL: `https://raw.githubusercontent.com/nordeste-rp/nordesterp-vehicles-images/refs/heads/main/vehicles/<modelo>.webp`.
- `vehicles/<modelo>.png` — mestre 1080x1080 RGBA (~290 KB). Fica só durante a transição para quem ainda pede `.png`.

`<modelo>` = o `index` do catálogo com a grafia **exata**: o raw do GitHub diferencia maiúsculas. Blindados
`16t`/`32t` usam a foto do carro base, copiada com o nome de cada variante (o git guarda arquivo igual uma vez só).

Geradas por `resources/[Ferramentas]/nrp_fotoveiculos` (fotografadas no jogo) e instaladas com
`tools/processa_fotos.py --instalar` (o `--webp-repo` só converte os `.png` que já estão aqui).

## clothes/

Fotos das roupas do `nrp_skinshop` (NordesteRP S4), em WebP 200x200 sem fundo.

- `clothes/{male|female}/{categoria}/{número}.webp` — número = o mesmo do menu da loja (originais do GTA build 3095
  primeiro, depois o pack `nordesteClothes2026_atual` na ordem das DLCs). Categorias: 1 máscaras, 3 mãos, 4 calças,
  5 mochilas, 6 sapatos, 7 acessórios, 8 camisas, 9 coletes, 10 adesivos, 11 jaquetas, p0 chapéus, p1 óculos,
  p2 brincos, p6 relógios, p7 pulseiras.
- `clothes/menu/{male|female}/{seção}.webp` — imagens das seções do menu.

Geradas por `resources/[Ferramentas]/nrp_fotoroupas` (peças do pack renderizadas offline; originais fotografadas
no jogo) e publicadas com `tools/publica_github.py`.
