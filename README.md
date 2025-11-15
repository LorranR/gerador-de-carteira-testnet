# gerador-de-carteira-testnet
O código gera automaticamente uma carteira Bitcoin na testnet usando padrões HD (Hierarchical Deterministic). Ele faz isso em etapas:

Gera um mnemonic (seed de 12 palavras)
— É a frase que permite restaurar a carteira.

Converte o mnemonic em uma seed criptográfica.

Cria a carteira HD raiz (BIP32).

Deriva um caminho específico (BIP49 → carteira SegWit compatível em testnet):
"m/49'/1'/0'/0/0"

Gera a chave pública e chave privada do endereço derivado.

Cria o endereço Bitcoin de recebimento usando a chave pública.

Exibe na tela:

O endereço Bitcoin

A chave privada (WIF)

A seed (mnemonic)
