# **Sound-to-Onomatopoeia Transcription Dataset**

The **Sound-to-Onomatopoeia Transcription Dataset** provides descriptive sentences using onomatopoeic expressions for each non-speech sound sample. Each sound sample is annotated by nine Korean listeners, capturing how the sounds are perceived by individuals. 

This dataset was created to develop a sound-to-onomatopoeia transcription model, which automatically transcribes non-speech sounds into onomatopoeic descriptions, reflecting various nuances and feelings associated with these sounds. It can be utilized in a range of research and application fields, including:
- Non-speech sound captioning for accessibility
- Textual sound effects
- Sound retrieval
- Sound synthesis, and more.

---

## **Description**
 
- **Category Information** : The dataset uses categories derived from the **Firat ESC50 dataset** [1].  Audio files can be downloaded here: [https://www.kaggle.com/datasets/buraktaci/firat-esc50](https://www.kaggle.com/datasets/buraktaci/firat-esc50)) Categories marked with an asterisk (*) were excluded from data collection. Below is the list of categories:

| **No.** | **Category**               | **No.** | **Category**               |
|---------|----------------------------|---------|----------------------------|
| 1*      | Man speaking               | 26      | Chopping food             |
| 2       | Flushing toilet           | 27      | Telephone dialing         |
| 3       | Pouring liquid            | 28*     | Girl speaking             |
| 4       | Tooth-brushing            | 29      | Car horn                  |
| 5*      | Woman speaking            | 30      | Writing                   |
| 6       | Car accelerating          | 31      | Computer startup sound    |
| 7       | Biting and chewing        | 32*     | Background speech         |
| 8       | Laughing                  | 33      | Songbird                  |
| 9       | Typing                    | 34      | Pouring water             |
| 10      | Car engine starting       | 35*     | Pop song                  |
| 11      | Running water             | 36      | Water boiling             |
| 12      | Breathing                 | 37*     | Guitar                    |
| 13      | Keys jangling             | 38      | Coughing                  |
| 14      | Dishes clanking           | 39      | Crumpling paper           |
| 15      | Ringtone                  | 40      | Siren                     |
| 16      | Microwave                 | 41      | Splashing water           |
| 17      | Dog barking               | 42*     | Computer speech           |
| 18      | Walking on a hard surface | 43      | Alarm clock               |
| 19      | Road traffic              | 44      | Walking with heels        |
| 20      | Zipper                    | 45      | Vacuum                    |
| 21      | Cellphone vibrating       | 46      | Wind                      |
| 22      | Water dripping            | 47*     | Boy speaking              |
| 23      | Scratching                | 48      | Chair rolling             |
| 24      | Car windows               | 49*     | Rock song                 |
| 25      | Telephone ringing         | 50      | Door knocking             |

- **Number of Samples:** During annotation, some annotations were missing due to problems with inaudible or low-volume sounds. To ensure each sample had the same number of annotated candidates, samples with missing annotations were removed from the dataset. As a results, a total of 7,962 samples were collected, each with five onomatopoeic expression candidate.

- **Dataset Details**: Each row in the dataset csv file includes the following fields:

| **Field**              | **Description**                                                                                      | **Example**               |
|------------------------|------------------------------------------------------------------------------------------------------|---------------------------|
| `audio_file`           | Name of the audio file, identical to the Firat ESC50 dataset.                                        | `10_ (13).mp3`            |
| `class`                | Sound category.                                                                                     | `10`                      |
| `id`                   | Sound clip index within the sound category.                                                         | `13`                      |
| `candidate1_ko` ~ `candidate5_ko` | 1 to 5 onomatopoeic description candidates (Korean).                                               | `칭 칙 치 치 부 르 르 릉`  |
| `candidate1_en` ~ `candidate5_en` | 1 to 5 onomatopoeic description candidates (English, converted to Latin alphabets using transliteration tools [2]). | `CHING CHIK CHI CHI BU REU REU REUNG` |

---

## **Citation**
If you use the **Sound-to-Onomatopoeia Transcription Dataset** in your research, please cite the following paper:

```bibtex
[bibtex here...]
```

---

## **References**
1. Taşcı, B., Acharya, M. R., Barua, P. D., Yildiz, A. M., Gun, M. V., Keles, T., ... & Tuncer, T. (2022). A new lateral geniculate nucleus pattern-based environmental sound classification using a new large sound dataset. *Applied Acoustics*, 196, 108897.  
2. Transliteration Tool: [https://github.com/elibooklover/Transliter](https://github.com/elibooklover/Transliter)

---

## **Contact**
For any questions about the dataset, please feel free to reach out:  
**JooYeong Kim**  
**Email:** [scijspirit@gmail.com](mailto:scijspirit@gmail.com)

