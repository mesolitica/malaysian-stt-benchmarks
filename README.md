# malaysian-stt-benchmarks

Benchmarking Malaysian Speech-to-Text models, HuggingFace space at https://huggingface.co/spaces/mesolitica/malaysian-stt-leaderboard

## Dataset

📈 We evaluate models based on 3 datasets,

1. Malaya-Speech test set, Malay language, https://huggingface.co/datasets/huseinzol05/malaya-speech-stt-test-set/tree/main/malaya-speech
2. Fleurs MS-MY test set, Malay language, https://huggingface.co/datasets/huseinzol05/malaya-speech-stt-test-set/tree/main/fleurs-ms-my
3. IMDA TTS first 700 audio files, English language but with Manglish slang, https://huggingface.co/datasets/mesolitica/IMDA-TTS

## Heavy postprocess test set

1. We filtered test set that contain numbers because malaya-speech transducer trained on normalized numbers.
2. We lower case because malaya-speech transducer trained on lower case.
3. We removed punctuation because malaya-speech transducer trained without punctuation.