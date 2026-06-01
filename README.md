# cooking-verb-translation-dataset

© 2026, Itsuki Takefuji, Kazuyoshi Takata, Isao Goto, and Takashi Ninomiya, Ehime University

This repository provides an English-Japanese dataset for verb translation in cooking procedure videos.

## Overview

This dataset was constructed to evaluate the translation of polysemous English verbs in cooking procedures.
In cooking instructions, the appropriate Japanese translation of a verb often depends not only on the text but also on the visual cooking process. For example, verbs such as *cook*, *boil*, *fry*, *spread*, and *toss* may require different Japanese translations depending on the ingredients, utensils, and actions shown in the video.

The dataset contains English cooking instructions, Japanese reference translations, video IDs, and temporal segment information. It is intended for research on machine translation, multimodal machine translation, and cooking procedure understanding.

## Dataset Description

The dataset is based on cooking procedure video segments. Each entry contains an English instruction, its Japanese translation, the corresponding video ID, and the start and end times of the segment.

The dataset is provided in CSV format.

### Files

```text
train.csv
test.csv
```

Each CSV file contains the following columns:

| Column     | Description                    |
| ---------- | ------------------------------ |
| `en`       | English cooking instruction    |
| `ja`       | Japanese reference translation |
| `video_id` | YouTube video ID               |
| `start`    | Start time of the segment      |
| `end`      | End time of the segment        |

## License

This dataset is released under the MIT License.

Please note that this dataset does not include raw video files.
The copyrights of the original videos belong to their respective owners.
Users are responsible for checking the copyright and usage conditions of the original videos when using them.

## Citation

If you use this dataset, please cite this repository.

```bibtex
@misc{takefuji2026cookingverbtranslation,
  title        = {Cooking Verb Translation Dataset},
  author       = {Itsuki Takefuji and Kazuyoshi Takata and Isao Goto and Takashi Ninomiya},
  institution  = {Ehime University},
  howpublished = {\url{https://github.com/take308/cooking-verb-translation-dataset}},
  year         = {2026}
}
```

## Acknowledgment

This dataset was constructed as part of research on English-Japanese translation of cooking procedures using text, image, and video information.
