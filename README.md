# YueDanPing
reliable evalution for LLM foundation models monthly.
It is not wide or deep, but faithfull. 

## evaluation methord
train on older corpus, evaluate on similar fresh corpus.

## result
* perplexity: lower is better

**The results depend on tokenizer and corpus.**

### result on chinaxiv-20240316
| **model**                                  | **params**      | **eval#2023** | **eval#2024** | **lora#2024** |
|--------------------------------------------|-----------------|---------------|---------------|---------------|
| Aquila2-7B                                 | 7,295,537,152   | 28.84825      | 30.05213      | -2            |
| Atom-7B                                    | 7,028,740,096   | 10.84875      | 11.1219       | 9.653549      |
| Baichuan2-7B-Base                          | 7,523,864,576   | 9.633932      | 9.881991      | 9.172034      |
| bloom-3b                                   | 3,002,557,440   | 15.17265      | 15.07577      | -2            |
| bloom-560m                                 | 559,214,592     | 28.04417      | 28.24155      | -2            |
| bloom-7b1                                  | 7,084,744,704   | 13.13629      | 12.95031      | 11.75081      |
| bloomz-3b                                  | 3,002,557,440   | 19.18721      | 19.05911      | -2            |
| bloomz-560m                                | 559,214,592     | 38.77743      | 37.65724      | -2            |
| bloomz-7b1                                 | 7,069,016,064   | 15.38627      | 15.14769      | -2            |
| BlueLM-7B-Base                             | 7,316,254,720   | 4422.868      | 32602.13      | 9.508107      |
| CodeLlama-7b-hf                            | 6,738,546,688   | 6.23645       | 5.090561      | -2            |
| DeciLM-7B                                  | 7,064,135,680   | 9.109229      | 9.253548      | 5.42167       |
| deepseek-coder-6.7b-base                   | 6,740,512,768   | 10.13893      | 8.666569      | -2            |
| deepseek-llm-7b-base                       | 6,929,104,896   | 10.22729      | 9.053343      | 8.246095      |
| falcon-7b                                  | 6,938,039,168   | 15.96314      | 15.00928      | 5.251349      |
| gemma-2b                                   | 2,506,172,416   | 22.85805      | 21.66038      | -2            |
| gemma-7b                                   | 8,537,680,896   | 64448108      | 3452662       | -2            |
| gpt-neo-1B3                                | 1,322,653,696   | 5.645107      | 4.923238      | 4.074434      |
| gpt-neo-2.7B                               | 2,663,104,000   | 5.131865      | 4.469001      | 3.717085      |
| internlm2-1_8b                             | 1,897,731,072   | 13.71936      | 13.92764      | 11.61148      |
| internlm2-7b                               | 7,737,708,544   | 15.53388      | 13.58698      | -2            |
| internlm2-base-7b                          | 7,757,356,032   | 14.93517      | 13.79963      | 8.9917        |
| internlm2-chat-1_8b                        | 1,889,110,016   | 14.72408      | 14.79291      | -2            |
| internlm2-chat-1_8b-sft                    | 1,889,110,016   | 15.0498       | 15.03722      | -2            |
| internlm2-chat-7b                          | 7,737,708,544   | 12.99174      | 12.57081      | -2            |
| internlm2-chat-7b-sft                      | 7,737,708,544   | 13.12358      | 12.65255      | -2            |
| LiteLlama-460M-1T                          | 465,863,680     | 8.093007      | 7.877329      | 5.220462      |
| Llama-2-7b-ms                              | 6,758,404,096   | 5.658247      | 4.869427      | 3.941072      |
| miniCPM-bf16                               | 2,738,520,576   | 16.34689      | 14.97825      | 12.24414      |
| Mistral-7B-v0.1                            | 7,262,703,616   | 6.62113       | 5.951056      | 4.954599      |
| Mistral-7B-v0.2-hf                         | 7,262,703,616   | 6.639457      | 6.099373      | 5.008702      |
| nlp_polylm_qwen_7b_text_generation         | 7,721,324,544   | 10.40996      | 9.785966      | -2            |
| open_llama_7b_v2                           | 6,758,404,096   | 7.188848      | 6.839469      | 5.625202      |
| opt-125                                    | 126,566,400     | 16.98976      | 14.58948      | 7.252155      |
| opt-1b3                                    | 1,322,835,968   | 9.679114      | 8.719473      | 5.026912      |
| phi-2                                      | 2,790,169,600   | 6.029123      | 5.085429      | 3.810656      |
| pythia-1b                                  | 1,016,394,752   | 9.468149      | 8.68096       | 6.781975      |
| pythia-6.9b-deduped                        | 6,874,515,456   | 7.428262      | 6.775186      | 5.338256      |
| Qwen1.5-0.5B                               | 463,987,712     | 17.16793      | 16.73722      | -2            |
| Qwen1.5-1.8B                               | 1,836,828,672   | 13.736        | 13.41481      | -2            |
| Qwen1.5-4B                                 | 3,950,369,280   | 10.84552      | 10.98453      | -2            |
| Qwen1.5-7B                                 | 7,741,313,024   | 9.690842      | 9.650169      | 8.874974      |
| RedPajama-INCITE-7B-Base                   | 6,874,515,456   | 7.629296      | 7.155577      | 5.530655      |
| SOLAR-10.7B-v1.0                           | 10,731,524,096  | 7.291903      | 6.948421      | -2            |
| stablelm-2-1_6b                            | 1,652,084,736   | 8.696677      | 7.797069      | 6.426664      |
| stablelm-3b-4e1t                           | 2,795,443,200   | 6.662487      | 5.92779       | -2            |
| TinyLlama-1.1B-intermediate-step-1431k-3T  | 1,106,356,224   | 5.714551      | 6.088251      | 4.81858       |
| TinyLlama-1.1B-intermediate-step-240k-503b | 1,100,048,384   | 8.576144      | 7.758241      | -2            |
| xgen-7b-4k-base                            | 6,915,690,496   | 4.008608      | 3.40011       | 2.998445      |
| XVERSE-7B                                  | 7,319,834,624   | 4.83116       | 4.58671       | 4.318017      |
| Yi-6B                                      | 6,079,188,992   | 10.12376      | 9.31675       | 8.658336      |
| Yi-9B                                      | 8,829,407,232   | 9.166134      | 8.575208      | -2            |
### result on UN_meeting_records-20240313
| **model**                                  | **params**      | **eval#2023** | **eval#2024** | **lora#2024** |
|--------------------------------------------|-----------------|---------------|---------------|---------------|
| Aquila2-7B                                 | 7,295,537,152   | 13.23194      | 14.2388       | -2            |
| Atom-7B                                    | 7,028,740,096   | 7.563231      | 7.694059      | 5.123826      |
| Baichuan2-7B-Base                          | 7,523,864,576   | 5.680863      | 5.859728      | 4.317772      |
| bloom-3b                                   | 3,002,557,440   | 17.16893      | 18.31615      | -2            |
| bloom-560m                                 | 559,214,592     | 31.32614      | 33.52478      | -2            |
| bloom-7b1                                  | 7,084,744,704   | 14.64726      | 15.65386      | 9.649741      |
| bloomz-3b                                  | 3,002,557,440   | 27.93955      | 29.93702      | -2            |
| bloomz-560m                                | 559,214,592     | 71.34502      | 74.60252      | -2            |
| bloomz-7b1                                 | 7,069,016,064   | 20.27191      | 21.66272      | -2            |
| BlueLM-7B-Base                             | 7,316,254,720   | 2623.164      | 2981.731      | 5.150276      |
| CodeLlama-7b-hf                            | 6,738,546,688   | 6.518433      | 6.54595       | -2            |
| DeciLM-7B                                  | 7,064,135,680   | 8.970972      | 9.404973      | 4.777601      |
| deepseek-coder-6.7b-base                   | 6,740,512,768   | 6.121032      | 6.172042      | -2            |
| deepseek-llm-7b-base                       | 6,929,104,896   | 6.341423      | 6.563469      | 4.84415       |
| falcon-7b                                  | 6,938,039,168   | 10.50134      | 10.51218      | 4.059371      |
| gemma-2b                                   | 2,506,172,416   | 26.98945      | 27.47368      | -2            |
| gemma-7b                                   | 8,537,680,896   | 212010.7      | 237804        | -2            |
| gpt-neo-1B3                                | 1,322,653,696   | 5.317842      | 5.54316       | 4.006921      |
| gpt-neo-2.7B                               | 2,663,104,000   | 4.938549      | 5.136749      | 3.731543      |
| internlm-7b                                | 7,321,948,160   | 8.905432      | 10.4819       | -2            |
| internlm2-1_8b                             | 1,897,731,072   | 6.4715        | 6.705878      | 4.656414      |
| internlm2-7b                               | 7,737,708,544   | 5.068815      | 5.323761      | -2            |
| internlm2-base-7b                          | 7,757,356,032   | 5.494074      | 5.806803      | 4.360255      |
| internlm2-chat-1_8b                        | 1,889,110,016   | 6.748659      | 6.968392      | -2            |
| internlm2-chat-1_8b-sft                    | 1,889,110,016   | 6.86979       | 7.086947      | -2            |
| internlm2-chat-7b                          | 7,737,708,544   | 5.157704      | 5.371175      | -2            |
| internlm2-chat-7b-sft                      | 7,737,708,544   | 5.205412      | 5.416234      | -2            |
| LiteLlama-460M-1T                          | 465,863,680     | 6.75242       | 7.085361      | 4.496822      |
| Llama-2-7b-hf                              | 6,738,415,616   | 6.01308       | 6.000242      | -2            |
| Llama-2-7b-ms                              | 6,758,404,096   | 6.01308       | 6.000242      | 4.43451       |
| llama-7b                                   | 6,738,415,616   | 6.621977      | 6.670652      | -2            |
| miniCPM-bf16                               | 2,738,520,576   | 7.68789       | 7.634563      | 5.155774      |
| Mistral-7B-v0.1                            | 7,262,703,616   | 5.729335      | 5.907934      | 4.432613      |
| Mistral-7B-v0.2-hf                         | 7,262,703,616   | 5.458835      | 5.971759      | 4.473939      |
| mpt-7b                                     | 6,649,286,656   | 6.702725      | 6.944704      | -2            |
| nlp_polylm_qwen_7b_text_generation         | 7,721,324,544   | 9.437592      | 9.554462      | -2            |
| OLMo-7B                                    | 6,888,095,744   | 6.715803      | 6.96987       | -2            |
| open_llama_7b                              | 6,738,415,616   | 4.312929      | 4.413033      | -2            |
| open_llama_7b_v2                           | 6,758,404,096   | 5.682711      | 5.685354      | 4.381169      |
| opt-125                                    | 126,566,400     | 10.24932      | 10.63422      | 6.212029      |
| opt-1b3                                    | 1,322,835,968   | 6.946911      | 7.239257      | 4.340449      |
| phi-2                                      | 2,790,169,600   | 6.174755      | 6.347548      | 4.222004      |
| pythia-1b                                  | 1,016,394,752   | 9.135172      | 9.400467      | 6.645516      |
| pythia-6.9b-deduped                        | 6,874,515,456   | 7.270118      | 7.595724      | 5.508924      |
| Qwen-1_8B-Llamafied                        | 1,836,877,824   | 24.27886      | 24.33767      | -2            |
| Qwen-7B                                    | 7,721,324,544   | 10.74675      | 10.98732      | -2            |
| Qwen1.5-0.5B                               | 463,987,712     | 21.61064      | 21.31525      | -2            |
| Qwen1.5-1.8B                               | 1,836,828,672   | 16.84911      | 16.8088       | -2            |
| Qwen1.5-4B                                 | 3,950,369,280   | 12.77069      | 12.96089      | -2            |
| Qwen1.5-7B                                 | 7,741,313,024   | 10.93399      | 11.17311      | 7.127         |
| RedPajama-INCITE-7B-Base                   | 6,874,515,456   | 6.886122      | 7.208492      | 5.174009      |
| SOLAR-10.7B-v1.0                           | 10,731,524,096  | 5.873455      | 6.077794      | -2            |
| stablelm-2-1_6b                            | 1,652,084,736   | 7.549793      | 7.764087      | 5.705255      |
| stablelm-3b-4e1t                           | 2,795,443,200   | 5.943108      | 6.226867      | -2            |
| TinyLlama-1.1B-intermediate-step-1431k-3T  | 1,106,356,224   | 7.344408      | 7.684493      | 5.352427      |
| TinyLlama-1.1B-intermediate-step-240k-503b | 1,100,048,384   | 9.416568      | 9.181088      | -2            |
| xgen-7b-4k-base                            | 6,915,690,496   | 3.995412      | 4.149289      | 3.126277      |
| XVERSE-7B                                  | 7,319,834,624   | 4.06319       | 4.151512      | 3.305972      |
| Yi-6B                                      | 6,079,188,992   | 5.493687      | 5.505545      | 4.235758      |
| Yi-9B                                      | 8,829,407,232   | 5.001919      | 5.063326      | -2            |

### result on wikinews-20240304
#### corpus  
news-202401/202402 from  wikinews-20240304
| language | 2023 | 2024-01 | 2024-02 |
|----------|------|---------|---------|
| Total    | 1670 | 120     | 74      |
| ar       | 20   | 33      | 4       |
| ca       | 26   | 1       | 0       |
| cs       | 307  | 31      | 16      |
| de       | 37   | 16      | 11      |
| el       | 1    | 0       | 0       |
| en       | 150  | 3       | 27      |
| eo       | 50   | 2       | 1       |
| es       | 77   | 21      | 4       |
| fa       | 7    | 0       | 0       |
| fi       | 1    | 0       | 1       |
| fr       | 315  | 12      | 10      |
| guw      | 679  | 1       | 0       |

#### result
| **model**                                  | **params**      | **eval#2024-01** | **eval#2024-02** | **lora#2024-01** | **lora#2024-02** |
|--------------------------------------------|-----------------|------------------|------------------|------------------|------------------|
| Aquila2-7B                                 | 7,315,525,632   | 16.30403         | 20.89646         | 6.065212         | 7.97123          |
| Atom-7B                                    | 7,028,740,096   | 5.575283         | 7.550279         | 4.573611         | 6.4228           |
| Baichuan2-7B-Base                          | 7,523,864,576   | 4.359303         | 5.794551         | 3.755924         | 5.202254         |
| bloom-3b                                   | 3,012,387,840   | 22.90577         | 31.64106         | 15.83741         | 23.881           |
| bloom-560m                                 | 562,360,320     | 53.86382         | 80.3743          | 35.75742         | 58.1996          |
| bloom-7b1                                  | 7,084,744,704   | 18.33257         | 24.13478         | 12.78142         | 18.5073          |
| bloomz-3b                                  | 3,012,387,840   | 35.71364         | 52.68064         | 17.99012         | 27.33712         |
| bloomz-560m                                | 562,360,320     | 82.51425         | 123.9445         | 41.25399         | 67.0926          |
| bloomz-7b1                                 | 7,084,744,704   | 24.69381         | 35.01303         | 13.94318         | 20.42104         |
| BlueLM-7B-Base                             | 7,316,254,720   | 3411.778         | 427.2565         | 5.219351         | 6.107629         |
| chatglm3-6b-base                           | 6,258,407,424   | 8.133553         | 11.02375         | 4.082908         | 5.597171         |
| CodeLlama-7b-hf                            | 6,758,535,168   | 5.265539         | 7.133512         | 4.422488         | 6.193972         |
| DeciLM-7B                                  | 7,064,135,680   | 7.241643         | 9.448154         | 4.339353         | 5.838205         |
| deepseek-coder-6.7b-base                   | 6,760,501,248   | 4.835029         | 7.916848         | 4.023368         | 6.695955         |
| deepseek-llm-7b-base                       | 6,929,104,896   | 4.610202         | 6.132427         | 3.960884         | 5.419725         |
| falcon-7b                                  | 6,938,039,168   | 15.09715         | 23.14824         | 6.82834          | 10.75367         |
| gemma-2b                                   | 2,515,978,240   | 23.33773         | 23.34022         | 8.73191          | 10.06568         |
| gemma-7b                                   | 8,562,682,880   | 503563.5         | 1415642          | 7.880434         | 9.012646         |
| gpt-neo-1B3                                | 1,322,653,696   | 6.717628         | 10.6243          | 5.811638         | 9.488335         |
| gpt-neo-2.7B                               | 2,663,104,000   | 5.984828         | 9.206106         | 5.09842          | 8.070748         |
| internlm-7b                                | 7,341,936,640   | 15.07735         | 12.5624          | 11.58088         | 10.66008         |
| internlm2-1_8b                             | 1,897,731,072   | 8.192929         | 13.84612         | 6.106452         | 10.48959         |
| internlm2-7b                               | 7,757,356,032   | 5.520153         | 8.289825         | 4.187122         | 6.437863         |
| internlm2-base-7b                          | 7,757,356,032   | 5.231546         | 7.953677         | 3.979664         | 6.262898         |
| internlm2-chat-1_8b                        | 1,897,731,072   | 8.374632         | 14.45481         | 6.21047          | 10.88569         |
| internlm2-chat-1_8b-sft                    | 1,897,731,072   | 8.588778         | 14.94404         | 6.216262         | 10.90602         |
| internlm2-chat-7b                          | 7,757,356,032   | 5.429047         | 7.890384         | 4.251997         | 6.723232         |
| internlm2-chat-7b-sft                      | 7,757,356,032   | 5.541009         | 8.056338         | 4.267017         | 6.705608         |
| LiteLlama-460M-1T                          | 465,863,680     | 9.086187         | 14.09878         | 7.409269         | 11.82525         |
| Llama-2-7b-hf                              | 6,758,404,096   | 4.675434         | 6.207275         | 3.931474         | 5.357683         |
| Llama-2-7b-ms                              | 6,758,404,096   | 4.675434         | 6.207275         | 3.931631         | 5.360066         |
| llama-7b                                   | 6,758,404,096   | 4.96496          | 6.767419         | 4.148877         | 5.791437         |
| miniCPM-bf16                               | 2,738,520,576   | 8.32307          | 11.67591         | 6.262321         | 9.155216         |
| Mistral-7B-v0.1                            | 7,262,703,616   | 4.250147         | 5.588682         | 3.623107         | 4.903256         |
| mpt-7b                                     | 6,649,286,656   | 7.35285          | 9.474119         | -1               | -1               |
| nlp_polylm_qwen_7b_text_generation         | 7,739,215,872   | 6.547418         | 7.270501         | 5.377188         | 6.328094         |
| OLMo-7B                                    | 6,888,095,744   | 7.329988         | 9.873527         | -1               | -1               |
| open_llama_7b                              | 6,758,404,096   | 3.274803         | 5.478099         | 2.874587         | 4.789103         |
| open_llama_7b_v2                           | 6,758,404,096   | 4.884668         | 6.051518         | 4.108351         | 5.270462         |
| opt-125                                    | 126,566,400     | 14.23733         | 24.8076          | 11.9095          | 21.40656         |
| opt-1b3                                    | 1,322,835,968   | 7.649281         | 11.14465         | 6.33929          | 9.609758         |
| phi-2                                      | 2,790,169,600   | 9.475558         | 16.74762         | 7.661525         | 13.45879         |
| pythia-1b                                  | 1,016,394,752   | 9.91897          | 13.5123          | 8.083432         | 11.70023         |
| pythia-6.9b-deduped                        | 6,874,515,456   | 7.26527          | 9.79727          | 5.738915         | 8.085229         |
| Qwen-1_8B-Llamafied                        | 1,844,373,504   | 28.92216         | 19.72609         | 11.91706         | 12.74216         |
| Qwen-7B                                    | 7,739,215,872   | 8.753631         | 7.797002         | 6.987481         | 6.807241         |
| Qwen1.5-0.5B                               | 467,772,416     | 21.22331         | 20.7434          | 15.96482         | 17.05816         |
| Qwen1.5-1.8B                               | 1,844,324,352   | 14.68596         | 14.3309          | 11.14278         | 11.76543         |
| Qwen1.5-4B                                 | 3,966,016,000   | 10.88744         | 10.18894         | 8.417567         | 8.67093          |
| Qwen1.5-7B                                 | 7,741,313,024   | 8.196657         | 8.256778         | 6.501196         | 7.086949         |
| RedPajama-INCITE-7B-Base                   | 6,874,515,456   | 5.997423         | 7.708963         | 5.021287         | 6.759973         |
| SOLAR-10.7B-v1.0                           | 10,762,981,376  | 4.199552         | 5.488511         | 3.459426         | 4.673364         |
| stablelm-2-1_6b                            | 1,652,084,736   | 6.560932         | 8.018926         | 5.511056         | 7.038959         |
| stablelm-3b-4e1t                           | 2,807,960,576   | 5.56371          | 6.910879         | 4.729144         | 6.127542         |
| TinyLlama-1.1B-intermediate-step-240k-503b | 1,106,356,224   | 8.920971         | 13.49263         | 7.127494         | 10.63824         |
| xgen-7b-4k-base                            | 6,915,690,496   | 4.194388         | 6.011444         | 3.612002         | 5.30681          |
| XVERSE-7B                                  | 7,319,834,624   | 3.194532         | 3.67341          | 2.782692         | 3.337815         |
| Yi-6B                                      | 6,079,188,992   | 4.457659         | 6.661217         | 3.735765         | 5.724027         |
| Yi-9B                                      | 8,856,637,440   | 4.042195         | 6.075996         | 3.429222         | 5.222183         |
| Yuan2-2B-hf                                | 2,097,768,448   | 67.75841         | 130.9332         | 17.67953         | 35.89121         |

### result on wikinews-20240122
#### corpus 
news-202401 from  wikinews-20240122
#### result
| Foundation Models                          | just eval | train only lora | train with byt5 tokenizer |   |
|--------------------------------------------|-----------|-----------------|---------------------------|---|
| deepseek-llm-7b-base                       | 4.418595  | 2.775576        | 2.435999                  |   |
| Llama-2-7b-hf                              | 4.496019  | 2.775896        | 2.756618                  |   |
| Yi-6B                                      | 5.031991  | 2.996905        | 2.367179                  |   |
| CodeLlama-7b-hf                            | 5.087177  | 3.045621        | 2.888906                  |   |
| deepseek-coder-6.7b-base                   | 5.15121   | 3.079392        | 2.519493                  |   |
| llama-7b                                   | 5.287015  | 3.155645        | 2.37461                   |   |
| TinyLlama-1.1B-intermediate-step-240k-503b | 8.20445   | 4.419586        | 2.628365                  |   |

