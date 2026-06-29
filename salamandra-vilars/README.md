# Salamandra · Els Vilars d'Arbeca i els ibers

Corpus en català per afinar (fine-tuning) el model **Salamandra** (BSC) sobre la
fortalesa ibèrica dels **Vilars d'Arbeca** i els **ibers** de la península Ibèrica.

| Fitxer | Contingut | Format |
|--------|-----------|--------|
| `sft_train.jsonl` | 256 parelles instrucció/resposta (entrenament) | `{"messages":[system,user,assistant]}` |
| `sft_validation.jsonl` | 28 parelles (validació, sense fuga) | `{"messages":[...]}` |
| `corpus_preentrenament.jsonl` | 112 passatges de text pla (injecció de coneixement) | `{"text":"..."}` |
| `corpus_instruccions.jsonl` | SFT original complet (59 parelles) | `{"messages":[...]}` |

Tots UTF-8, JSON Lines. Pensats per a SFT amb 🤗 TRL (LoRA/QLoRA).
