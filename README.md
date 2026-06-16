# cooking-verb-translation-dataset

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
This project includes data derived from the YouCook2-JP and YouCook2 datasets.

- **YouCook2**
  - **Source**: http://youcook2.eecs.umich.edu/
  - **License**: MIT License
  - **License file**: [licenses/LICENSE_YOUCOOK2.txt](licenses/LICENSE_YOUCOOK2.txt)
  - **Original license URL**: http://youcook2.eecs.umich.edu/static/YouCookII/LICENSE_YOUCOOK2.txt

- **YouCook2-JP**
  - **Source**: https://github.com/nlab-mpg/YouCook2-JP/
  - **License**: MIT License
  - **License file**: [licenses/LICENSE_YouCook2-JP.txt](licenses/LICENSE_YouCook2-JP.txt)
  - **Original license URL**: https://github.com/nlab-mpg/YouCook2-JP

Modified by Itsuki Takefuji, Kazuyoshi Takata, Isao Goto, and Takashi Ninomiya, Ehime University (c) 2026.

Released under the [MIT License](LICENSE.txt).

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
