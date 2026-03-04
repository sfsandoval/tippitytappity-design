# tippitytappity-design

tippitytappity is a program to practice typing


## Data model


```mermaid
classDiagram
  
  class Phrase{
        - id: int
        - text: string
        - difficulty: int
        + phrase(id: int, text: string, difficulty: int)
        + get_id() int
        + get_text() string
        + get_difficulty() int

  }
  class PhraseBank{
        - phrases vector~Phrase~
        + PhraseBank()
        + add_phrase(p: Phrase)
        + size() int
        + get_phrase(index: int) Phrase
        + get_random_phrase() Phrase
        + load_default_phrases()
  }
class type_speed{
  - speed: int
  +get_speed() int
}



```
