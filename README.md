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

class accuracy{
  - words: int
  - words_correct int
  - accuracy int
  +get_accuracy() int

}

class users{
  - user_id: int
  - users vector~user~
  + get_user(users vector~user~, user_id:int) int
}

class history{
  - score: int
  - tests vector~get_accuracy()~

  +get_test_history(tests) int
}

```
