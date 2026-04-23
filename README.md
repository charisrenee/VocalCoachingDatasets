# Vocal Datasets

Starter registry of vocal and singing datasets.

Source of truth for the table below: `datasets.csv`

## Columns

- `name`
- `year`
- `task`
- `scale`
- `annotations`
- `data_types`
- `owner`
- `language`
- `access`
- `license`
- `paper`
- `dataset_url`
- `notes`

## Datasets

### Recommended

| name | year | task | scale | annotations | access | dataset_url | notes |
|---|---|---|---|---|---|---|---|
| 10KSinging | 2021 | singing assessment | 9,756 songs, 190 singers | overall quality rating | request | not specified | recommended assessment dataset from the shortlist |
| Sing-MD | 2025 | expert singing assessment | 1,000 clips | expert 4-dim scores: breath control; timbre quality; emotional expression; vocal technique | request | https://github.com/CarlWangChina/Singing-Aesthetic-Assessment | high-value if access is workable |
| PopBuTFy | 2022 | amateur vs professional singing comparison | multiple songs, paired recordings | parallel amateur/professional recordings of the same songs | open | not specified | recommended paired-performance dataset from the shortlist |
| VocalSet | 2018 | technique recognition | 10.1 hrs, 20 singers | 17 vocal techniques (vibrato, belt, breathy, etc.) | open | https://zenodo.org/records/1442513 | core dataset for vocal technique work |
| Annotated-VocalSet | 2022 | pitch / note supervision | extension of VocalSet | per-note technique labels | open | https://zenodo.org/records/7061507 | extends VocalSet with note annotations |
| GTSinger | 2024 | multi-task singing | 80.59 hrs, 9 languages | 5 techniques with controlled phoneme-level annotation | open | https://huggingface.co/datasets/GTSinger/GTSinger | broad foundation dataset |
| SingPAD | 2024 | sight-singing / learner modeling | 1,074 learners, longitudinal | knowledge-tracing interactions from SingMaster platform | request | https://github.com/itec-hust/singKT-dataset | no raw singing-audio focus, but strong for tutoring logic |

---

### Full Registry

| name | year | task | scale | annotations | data_types | owner | language | access | license | paper | dataset_url | notes |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 10KSinging | 2021 | singing assessment | 9,756 songs, 190 singers | overall quality rating | audio; overall quality rating | not specified | not specified | request | check source terms | not specified | not specified | recommended assessment dataset from the shortlist |
| Sing-MD | 2025 | expert singing assessment | 1,000 clips | expert 4-dim scores: breath control; timbre quality; emotional expression; vocal technique | audio; 4-dim expert scores; text critiques | Zhejiang University authors | Mandarin | request | verify terms | https://github.com/CarlWangChina/Singing-Aesthetic-Assessment | https://github.com/CarlWangChina/Singing-Aesthetic-Assessment | high-value if access is workable |
| PopBuTFy | 2022 | amateur vs professional singing comparison | multiple songs, paired recordings | parallel amateur/professional recordings of the same songs | paired amateur/professional recordings | not specified | not specified | open | check source terms | not specified | not specified | recommended paired-performance dataset from the shortlist |
| VocalSet | 2018 | technique recognition | 10.1 hrs, 20 singers | 17 vocal techniques (vibrato, belt, breathy, etc.) | audio; singer labels; technique labels; vowels | Northwestern University | English | open | check Zenodo terms | https://zenodo.org/records/1492453 | https://zenodo.org/records/1442513 | core dataset for vocal technique work |
| Annotated-VocalSet | 2022 | pitch / note supervision | extension of VocalSet | per-note technique labels | audio-aligned F0; note onsets; note offsets; MIDI pitch; lyrics | Maynooth University | English | open | check Zenodo terms | https://zenodo.org/records/7061507 | https://zenodo.org/records/7061507 | extends VocalSet with note annotations |
| GTSinger | 2024 | multi-task singing | 80.59 hrs, 9 languages | 5 techniques with controlled phoneme-level annotation | audio; paired speech; phoneme alignment; technique labels; style labels; music scores | Zhejiang University | multilingual | open | dataset terms | https://huggingface.co/papers/2409.13832 | https://huggingface.co/datasets/GTSinger/GTSinger | broad foundation dataset |
| SingPAD | 2024 | sight-singing / learner modeling | 1,074 learners, longitudinal | knowledge-tracing interactions from SingMaster platform | records; note correctness; concept mappings; pitch/rhythm evaluations | HUST / SingMaster | not specified | request | check source terms | https://zenodo.org/records/12729828 | https://github.com/itec-hust/singKT-dataset | no raw singing-audio focus, but strong for tutoring logic |
| Lyra-SA | not specified | singing assessment | not specified | audio; ratings; MIDI; lyrics | audio; ratings; MIDI; lyrics | Tencent / WeSing / Tianqin Music Lab | Mandarin | open | check source terms | https://lyracobar.y.qq.com/singvoicedataset_en.html | https://lyracobar.y.qq.com/singvoicedataset_en.html | good starting dataset for full-song scoring |
| SingEval | not specified | singing assessment | not specified | annotations; ratings | annotations; ratings | SingEval authors + DAMP audio | English | open annotations / restricted audio | mixed | https://github.com/chitralekha18/SingEval | https://github.com/chitralekha18/SingEval | depends on DAMP for audio |
| DAMP-VP1k | not specified | karaoke singing | not specified | audio; metadata; singer ids | audio; metadata; singer ids | Smule | multilingual | restricted | Smule research terms | https://zenodo.org/records/2533419 | https://zenodo.org/records/2533419 | useful source audio for singing assessment |
| PESnQ-DS | not specified | singing assessment | not specified | audio; overall score; intonation; rhythm; vibrato; timbre; pronunciation | audio; overall score; intonation; rhythm; vibrato; timbre; pronunciation | NUS researchers | English | limited / paper-linked | check source terms | https://www.cambridge.org/core/journals/apsipa-transactions-on-signal-and-information-processing/article/technical-framework-for-automatic-perceptual-evaluation-of-singing-quality/5F6AECB907FE842481D070850EDF1EFA | https://smcnus.comp.nus.edu.sg/archive/pdf/2017-2018/2018_pesnq-apsipa-transactions.pdf | fine-grained feedback labels |
| SPED | not specified | sight-singing evaluation | not specified | audio; pitch score sequences; rhythm score sequences; score metadata | audio; pitch score sequences; rhythm score sequences; score metadata | SPED authors | not specified | paper says open | check source terms | https://doi.org/10.1109/ICASSP49660.2025.10889301 | https://doi.org/10.1109/ICASSP49660.2025.10889301 | large learner dataset |
| Vocadito | not specified | pitch tracking | not specified | audio; F0; note annotations; lyrics; language labels | audio; F0; note annotations; lyrics; language labels | Spotify + IRCAM | multilingual | open | check Zenodo terms | https://zenodo.org/records/5578807 | https://zenodo.org/records/5578807 | clean monophonic singing dataset |
| SingMOS | not specified | singing quality prediction | not specified | audio; MOS ratings | audio; MOS ratings | SingMOS authors | Mandarin, Japanese | open | check HF terms | https://huggingface.co/papers/2406.10911 | https://huggingface.co/datasets/TangRain/SingMOS | useful for perceived quality modeling |
| SingMOS-Pro | not specified | multi-dimensional singing quality | not specified | audio; overall; lyrics; melody ratings | audio; overall; lyrics; melody ratings | SingMOS-Pro authors | Mandarin, Japanese | open | check HF terms | https://huggingface.co/papers/2510.01812 | https://huggingface.co/datasets/TangRain/SingMOS-Pro | more detailed than SingMOS |
| MIR-1K | not specified | pitch / separation | not specified | audio; pitch contours; lyrics; vocal activity | audio; pitch contours; lyrics; vocal activity | National Taiwan University researchers | Mandarin | open | check source terms | http://mirlab.org/dataset/public/ | https://zenodo.org/records/3532216 | classic karaoke dataset |
| iKala | not specified | pitch / lyrics / separation | not specified | audio; F0; timestamped lyrics; vocal activity | audio; F0; timestamped lyrics; vocal activity | National Taiwan University researchers | Chinese pop | request | check source terms | http://mirlab.org/dataset/public/ | https://zenodo.org/records/3532214 | widely used benchmark |
| MedleyDB | not specified | melody / stems | not specified | multitrack audio; stems; melody annotations | multitrack audio; stems; melody annotations | MedleyDB collaborators | mixed | open | CC BY-NC-SA | http://medleydb.weebly.com/ | http://medleydb.weebly.com/ | useful support dataset, not singing-only |
| MUSDB18 | not specified | source separation | not specified | audio stems | audio stems | SigSep / MUSDB creators | mixed | request | dataset terms | https://zenodo.org/records/1117372 | https://zenodo.org/records/1117372 | for accompaniment removal pipelines |
| DALI | not specified | lyrics alignment | not specified | lyrics alignments; melody info | lyrics alignments; melody info | DALI authors | mixed | open annotations | check repo terms | https://github.com/gabolsgabs/DALI | https://github.com/gabolsgabs/DALI | audio depends on YouTube availability |
| M4Singer | not specified | multi-singer singing | not specified | audio; note boundaries; phoneme alignment; MIDI; pitch; style labels | audio; note boundaries; phoneme alignment; MIDI; pitch; style labels | M4Singer authors | Mandarin | open | CC BY-NC | https://m4singer.github.io/ | https://m4singer.github.io/ | strong support dataset |
| OpenCPOP | not specified | SVS benchmark | not specified | audio; phoneme boundaries; MIDI; lyrics; TextGrid | audio; phoneme boundaries; MIDI; lyrics; TextGrid | OpenCPOP authors | Mandarin | open | CC BY-NC-ND | https://github.com/wenet-e2e/opencpop | https://wenet-e2e.github.io/opencpop/ | clean benchmark corpus |
| CSD | not specified | song alignment | not specified | audio; MIDI; grapheme/phoneme lyrics | audio; MIDI; grapheme/phoneme lyrics | CSD authors | Korean, English | open | check repo terms | https://github.com/equal-singer/CSD | https://github.com/equal-singer/CSD | simple aligned songs |
| NHSS | not specified | speech-to-singing | not specified | speech; singing; word annotations | speech; singing; word annotations | NUS researchers | English | open for research | check source terms | https://hltnus.github.io/NHSSDatabase/ | https://hltnus.github.io/NHSSDatabase/ | useful for pronunciation transfer ideas |
| NUS-48E | not specified | sung vs spoken | not specified | audio; phone annotations | audio; phone annotations | NUS | English | open | check source terms | https://smcnus.comp.nus.edu.sg/ | https://smcnus.comp.nus.edu.sg/ | small but useful alignment dataset |
| SingVERSE | not specified | singing enhancement | not specified | noisy-clean audio pairs | noisy-clean audio pairs | SingVERSE authors / Amphion | mixed | open | check HF terms | https://singverse.github.io/ | https://huggingface.co/datasets/amphion/SingVERSE | useful later for noisy practice recordings |
| SVQTD | not specified | vocal pedagogy attributes | not specified | audio; paralinguistic singing labels | audio; paralinguistic singing labels | SVQTD authors | likely classical vocal repertoire | public page | verify before use | https://yanzexu.xyz/SVQTD/ | https://yanzexu.xyz/SVQTD/ | interesting for pedagogy-oriented labels |
| Saarbruecken Voice Database | not specified | vocal health | not specified | voice recordings; healthy/pathological labels | voice recordings; healthy/pathological labels | Saarland University / Essen University Hospital | German | open | verify license | https://doi.org/10.1080/02699200701830869 | https://zenodo.org/records/16874898 | speech/clinical, not singing-specific |
| GRB assessment of Saarbruecken Voice Database | not specified | vocal quality labels | not specified | GRB labels | GRB labels | UdeA / UPM authors | German | open | verify license | https://doi.org/10.1109/JSTSP.2019.2956410 | https://zenodo.org/records/3550736 | add-on labels for Saarbruecken |
| SongEval | not specified | song aesthetics | not specified | audio; multi-dimensional ratings | audio; multi-dimensional ratings | ASLP Lab authors | English, Mandarin | open | check repo terms | https://github.com/ASLP-lab/SongEval | https://github.com/ASLP-lab/SongEval | includes vocal naturalness but is not vocal-only |
| STraDa | not specified | singer traits | not specified | audio; singer id; gender; age; language; genre | audio; singer id; gender; age; language; genre | STraDa authors | mixed | open | CC BY-NC | https://zenodo.org/records/10057434 | https://zenodo.org/records/10057434 | more singer-traits than coaching |
