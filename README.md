# Jōyō kanji

All jōyō kanji data scraped from [jisho.org](https://jisho.org)

```ts
type Kanji = {
    kanji: string;
    grade: 1 | 2 | 3 | 4 | 5 | 6 | 8 | 9 | 10 | null;
    jlpt: 1 | 2 | 3 | 4 | 5 | null;
    meanings: string[];
    kun: string[];
    on: string[];
    strokes: (string | number)[][];
    words: {
        word: [
            string,         // text
            string | null   // furigana
        ][];
        common: boolean;
        jlpt: 1 | 2 | 3 | 4 | 5 | null;
        meanings: {
            type: string;
            meaning: string;
        }[];
        sentences: {
            sentence: [
                string,         // text
                string | null   // furigana
            ][];
            translation: string;
        }[];
    }[];
};
```
