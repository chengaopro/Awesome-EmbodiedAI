# Awesome EmbodiedAI (still in construct) [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

We maintain a curated list of Awesome Embodied AI works. Currently, we include simulators, tasks and datasets in Embodied AI field. 
- Simulators help render images and simulate the behavior of agents, as if they are situated in an real world environment. 
- Datasets provide training data (e.g. navigation instructions) and ground truths (e.g. navigation trajectories). 

(Some simulator comes along with a dataset with the same name, so there might be duplicated names in different sections.)

Please feel free to pull requests or open an issue to add papers.

## Awesome companies

- [Covariant](https://covariant.ai/)
- [Mujin](https://www.mujin.co.jp/en/)
- [Righthand](https://www.righthandrobotics.com/)
- [Boston Dynamics](https://www.bostondynamics.com/)

## Awesome Labs

- [SVL](http://svl.stanford.edu/)

## Simulator

_Platform to simulate real world environments._

- Habitat-Simulator
  - Venue/Year: ICCV 2019 | [[paper]](https://arxiv.org/abs/1904.01201) [[code]](https://github.com/facebookresearch/habitat-sim) [[homepage]](https://aihabitat.org/)
  - Visual Content: Matterport3D, House3D, AI2-THOR, etc. (_partially realistic_)
  - Action Space: continuous
- AI2-THOR  
  - Venue/Year: Arxiv 2019 | [[paper]](https://arxiv.org/abs/1712.05474) [[code]](https://github.com/allenai/ai2thor) [[homepage]](https://ai2thor.allenai.org/)
  - Visual Content: AI2-THOR
  - Action Space: continuous
  - Interactive: Yes
- CHALET 
  - Venue/Year: Arxiv 2019 | [[paper]](https://arxiv.org/abs/1801.07357) [[code]](https://github.com/lil-lab/chalet)
  - Visual Content: CHALET
  - Action Space: continuous
  - Interactive: Yes
- Matterport3D 
  - Venue/Year: 3DV 2017 | [[paper]](https://arxiv.org/abs/1709.06158) [[code]](https://github.com/niessner/Matterport) [[homepage]](https://niessner.github.io/Matterport/) 
  - Visual Content: Matterport3D (realistic)
  - Action Space: graph based
- MINOS 
  - Venue/Year: CVPR 2017 | [[paper]](https://arxiv.org/abs/1712.03931) [[code]](https://github.com/minosworld/minos) [[homepage]](https://minosworld.github.io/)
  - Visual Content: SUNCG+Matterport3D (partially realistic)
  - Action Space: continuous
- Gibson 
  - Venue/Year: CVPR 2018 | [[paper]](https://arxiv.org/abs/1808.10654) [[code]](https://github.com/StanfordVL/GibsonEnv) [[homepage]](http://gibsonenv.stanford.edu/)
  - Visual Content: Gibson+2D3DS+Matterport3D (realistic)
  - Action Space: continuous
  - Interactive: Yes
- House3D 
  - Venue/Year: Arxiv 2018 | [[paper]](https://arxiv.org/abs/1801.02209) [[code]](https://github.com/facebookresearch/House3D)
  - Visual Content: SUNCG
  - Action Space: continuous
- SUNCG 
  - Venue/Year: CVPR 2017 | [[paper]](https://arxiv.org/abs/1611.08974) 
  - Visual Content: SUNCG
- HoME  
  - Venue/Year: NIPS 2017 | [[paper]](https://arxiv.org/abs/1711.11017) [[code]](https://github.com/ml-lab/home-platform)
  - Visual Content: SUNCG
  - language content: description of objects
  - Action Space: continuous
- VirtualHome  
  - Venue/Year: CVPR 2018 | [[paper]](https://arxiv.org/abs/1806.07011) [[code]](https://github.com/xavierpuigf/virtualhome) [homepage](http://virtual-home.org/) 
  - Visual Content: VirtualHome
  - Action Space: continuous
  - Interactive: Yes
- SceneNet RGB-D 
  - Venue/Year: ICCV 2017 | [[paper]](http://www.imperial.ac.uk/media/imperial-college/research-centres-and-groups/dyson-robotics-lab/jmccormac_etal_iccv2017.pdf) [[code]](https://github.com/jmccormac/pySceneNetRGBD) [[homepage]](https://robotvault.bitbucket.io/scenenet-rgbd.html)
  - Visual Content: SceneNet RGB-D
  - Action Space: continuous
  - Interactive: Yes

## Tasks

_Embodied task definitions._

[REVERIE](https://arxiv.org/abs/1904.10151) - requires an intelligent agent to correctly localize a remote target object (can not be observed at starting location) specified by a concise high-level natural language instruction.

[VLN](https://arxiv.org/abs/1711.07280) - requires an embodied agent to follow natural language instructions to navigate from a starting pose to a goal location.

[VNLA](https://arxiv.org/abs/1812.04155) - a grounded vision-language task where an agent with visual perception is guided via language to find objects in photorealistic indoor environments.

[EQA](https://arxiv.org/abs/1711.11543) - an agent is spawned at a random location in a 3D environment and asked a question. The agent must first intelligently navigate to explore the environment, gather necessary visual information through first-person (egocentric) vision, and then answer the question.

[IQA](https://arxiv.org/abs/1712.03316) - requires an agent to navigate around the scene, acquire visual understanding of scene elements, interact with objects (e.g. open refrigerators) and plan for a series of actions conditioned on the question.

[TOUCHDOWN](https://arxiv.org/abs/1811.12354) - requires an agent to first follow navigation instructions in a real-life visual urban environment, and then identify a location described in natural language to find a hidden object at the goal position.

## Dataset

_Embodied datasets built upon simulators._

- REVERIE _CVPR 2020_ based on Matterport3D [paper](https://arxiv.org/abs/1904.10151) [code](https://github.com/YuankaiQi/REVERIE) 
  - language content: navigation instructions
  - applicable tasks: REVERIE, VLN, referring expression
- R2R _CVPR 2018_ based on Matterport3D [paper](https://arxiv.org/abs/1711.07280) [homepage](https://bringmeaspoon.org/)
  - language content: navigation instructions
  - applicable tasks: VLN
- VNLA _CVPR 2019_ based on Matterport3D [paper](https://arxiv.org/abs/1812.04155) [code](https://github.com/debadeepta/vnla) 
  - language content: navigation instructions and assistance
  - applicable tasks: VNLA, VLN, referring expression
- HANNA _EMNLP 2019_ based on Matterport3D [paper](https://arxiv.org/abs/1909.01871) [code](https://github.com/khanhptnk/hanna)
  - language content: navigation instructions and assistance
  - applicable tasks: VNLA, VLN, referring expression
- CVDN _CoRL 2019_ based on Matterport3D [paper](https://arxiv.org/abs/1907.04957) [code](https://github.com/mmurray/cvdn/) [homepage](https://cvdn.dev/) 
  - language content: dialogues
  - applicable tasks: VNLA, VLN
- EQA _CVPR 2018_ based on House3D [paper](https://arxiv.org/abs/1711.11543) [code](https://github.com/facebookresearch/EmbodiedQA) [homepage](https://embodiedqa.org/)
  - language content: question-answer pairs
  - applicable tasks: EQA, VLN
- IQUADv1 _CVPR 2018_ based on AI2-THOR [paper](https://arxiv.org/abs/1712.03316) [code](https://github.com/danielgordon10/thor-iqa-cvpr-2018)
  - language content: question-answer pairs
  - applicable tasks: IQA, EQA, VLN
- TOUCHDOWN _CVPR 2019_ based on Google Street View [paper](https://arxiv.org/abs/1811.12354) [code](https://github.com/lil-lab/touchdown)
  - language content: navigation instructions
  - applicable tasks: TOUCHDOWN, VLN, referring expression
- Talk The Way _2018_ [paper](https://arxiv.org/abs/1807.03367) [code](https://github.com/facebookresearch/talkthewalk/)
  - visual content: manually captured neighborhoods of New York City
  - language content: navigation dialogues
  - applicable tasks: VNLA, VLN
- LANI & CHAI _2019_ based on CHALET [paper](https://arxiv.org/abs/1801.07357) [code](https://github.com/lil-lab/chalet)
  - language content: navigation instructions
  - applicable tasks: VLN
- Activity & ActivityPrograms _CVPR 2018_ [paper](https://arxiv.org/abs/1806.07011) [code](https://github.com/xavierpuigf/virtualhome) [homepage](http://virtual-home.org/) 
  - language content: task descriptions
  - applicable tasks: VLN
- Habitat _ICCV 2019_ [paper](https://arxiv.org/abs/1904.01201) [code](https://github.com/facebookresearch/habitat-sim) [homepage](https://aihabitat.org/) 
  - language content: navigation instructions, task descriptions, etc.
  - applicable tasks: IQA, EQA, VLN, language grounding, etc.
