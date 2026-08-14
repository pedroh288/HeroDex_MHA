# 1
Sim. Para o **HeroDex**, eu separaria os dois campos assim:

* **Tipo** → classificação da natureza da Individualidade.
* **Origem** → como aquela Individualidade chegou a existir/foi obtida pelo usuário.

### 🧬 Tipos de Individualidade

No universo de *My Hero Academia*, existem **3 tipos oficiais principais**:

| Tipo              | Japonês | O que significa                                           | Exemplos               |
| ----------------- | ------- | --------------------------------------------------------- | ---------------------- |
| **Emissão**       | 発動系     | O usuário produz, controla ou libera algum efeito/poder   | Explosion, One For All |
| **Transformação** | 変形系     | O usuário altera o próprio corpo temporariamente          | Hardening, Engine      |
| **Mutante**       | 異形系     | O corpo possui permanentemente características diferentes | Frog, Engine?*         |

* **Engine** é classificada como Mutante, apesar de poder parecer diferente à primeira vista.

#### Portanto, no seu template:

```yaml
Tipo: Emissão
```

ou

```yaml
Tipo: Transformação
```

ou

```yaml
Tipo: Mutante
```

---

## 🧬 Origens

Aqui eu faria uma classificação **do próprio HeroDex**, porque "origem" não é uma classificação oficial de Individualidades como os três tipos acima.

Sugestão:

| Origem           | Significado                                             |
| ---------------- | ------------------------------------------------------- |
| **Hereditária**  | Individualidade relacionada à herança genética dos pais |
| **Espontânea**   | Manifestou-se naturalmente no próprio indivíduo         |
| **Transferida**  | Recebida de outro indivíduo                             |
| **Artificial**   | Criada ou modificada artificialmente                    |
| **Roubo**        | Obtida através do roubo de uma Individualidade          |
| **Modificada**   | Individualidade original alterada artificialmente       |
| **Desconhecida** | Origem ainda não conhecida                              |

#### Exemplos

**Shoto:**

```yaml
Tipo: Mutante
Origem: Hereditária
```

**Bakugo:**

```yaml
Tipo: Emissão
Origem: Hereditária
```

**Deku / One For All:**

```yaml
Tipo: Emissão
Origem: Transferida
```

**All For One:**

```yaml
Tipo: Emissão
Origem: Desconhecida
```

---

#### ⚠️ Uma correção importante

Eu corrigiria uma coisa que falei anteriormente: **Half-Cold Half-Hot é uma Individualidade do tipo Emissão**, não "Híbrida". O fato de ela possuir gelo e fogo não cria uma quarta categoria oficial.

Para o HeroDex, eu recomendo manter **somente os três tipos oficiais**:

```yaml
Tipo: Emissão
Tipo: Transformação
Tipo: Mutante
```

E deixar `Origem` como uma classificação própria do seu banco.

Então seu template-base ficaria:

```yaml
---
Individualidade:
Nome original:
Nome em inglês:
Tipo:
Usuários:
Origem:
---
```

Isso é uma base bem melhor para depois transformar o HeroDex em um banco de dados real.
