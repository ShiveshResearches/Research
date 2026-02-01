## Experiment: Effect of Environmental and Hardware Factors on Speech Recognition

| Experiment ID | Environment        | Microphone Used        | Internet Quality | Speaking Pace | Attempts | Successful Detection | Misinterpretation | Key Observation |
|--------------|--------------------|------------------------|------------------|---------------|----------|----------------------|-------------------|-----------------|
| E1           | Noisy room         | Laptop built-in mic    | Stable           | Normal        | 5        | 2                    | 2                 | High failure rate due to background noise and poor mic quality |
| E2           | Noisy room         | Bluetooth headset      | Stable           | Normal        | 5        | 5                    | 2                 | External mic improved detection, but recognition errors remained |
| E3           | Quiet + noisy mix  | Bluetooth headset      | Stable           | Fast          | Multiple | Reduced              | Increased         | Fast speech increased misinterpretation |
| E4           | Quiet environment  | Bluetooth headset      | Poor             | Normal        | Multiple | Inconsistent         | Increased         | Poor internet caused delays and incorrect recognition |
| E5           | Quiet environment  | Bluetooth headset      | Stable           | Slow & clear  | Multiple | High                 | Low               | Slow, clear speech improved accuracy significantly |

### Analysis
The experiments indicate that speech recognition accuracy is influenced more by environmental and external factors than by code logic. Background noise and microphone quality primarily affect detection, while speaking pace and internet stability impact recognition accuracy. These results suggest that improving input quality and system conditions can significantly enhance performance without modifying the core algorithm.
