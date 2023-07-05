# Parameter List

**Parameters are options added to a prompt that change how an image generates. Parameters can change an image's Aspect Ratios, switch between Midjourney Model Versions, change which Upscaler is used, and lots more.**

Parameters are always added to the end of a prompt. You can add multiple parameters to each prompt.

![Example of how Midjourney parameters are used.](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ\_Parameters\_example.png)

Using an Apple device?

Many apple devices automatically change double hyphens (--) to an em-dash (—). Midjourney accepts both!



### Basic Parameters <a href="#basic-parameters" id="basic-parameters"></a>

#### Aspect Ratios

`--aspect`, or `--ar` Change the aspect ratio of a generation.

#### Chaos

`--chaos <number 0–100>` Change how varied the results will be. Higher values produce more unusual and unexpected generations.

#### No

`--no` Negative prompting, `--no plants` would try to remove plants from the image.

#### Quality

`--quality <.25, .5, 1, or 2>`, or `--q <.25, .5, 1, or 2>` How much rendering quality time you want to spend. The default value is 1. Higher values cost more and lower values cost less.

#### Seed

`--seed <integer between 0–4294967295>` The Midjourney bot uses a seed number to create a field of visual noise, like television static, as a starting point to generate the initial image grids. Seed numbers are generated randomly for each image but can be specified with the --seed or --sameseed parameter. Using the same seed number and prompt will produce similar ending images.

#### Stop

`--stop <integer between 10–100>` Use the `--stop` parameter to finish a Job partway through the process. Stopping a Job at an earlier percentage can create blurrier, less detailed results.

#### Style

`--style <4a, 4b or 4c>` Switch between versions of the Midjourney Model Version 4

#### Stylize

`--stylize <number>`, or `--s <number>` parameter influences how strongly Midjourney's default aesthetic style is applied to Jobs.

#### Uplight

`--uplight` Use an alternative "light" upscaler when selecting the U buttons. The results are closer to the original grid image. The upscaled image is less detailed and smoother.

#### Upbeta

`--upbeta` Use an alternative beta upscaler when selecting the U buttons. The results are closer to the original grid image. The upscaled image has significantly fewer added details.

#### Default Values (Model Version 4)

|                          | Aspect Ratio | Chaos | Quality     | Seed                       | Stop   | Style         | Stylize |
| ------------------------ | ------------ | ----- | ----------- | -------------------------- | ------ | ------------- | ------- |
| <p>Default Value<br></p> | 1:1          | 0     | 1           | Random                     | 100    | 4c            | 100     |
| <p>Range<br></p>         | 1:2–2:1      | 0–100 | .25 .5 or 1 | whole numbers 0–4294967295 | 10–100 | 4a, 4b, or 4c | 0–1000  |

#### Default Values (Model Version 5)

|                          | Aspect Ratio | Chaos | Quality      | Seed                       | Stop   | Stylize |
| ------------------------ | ------------ | ----- | ------------ | -------------------------- | ------ | ------- |
| <p>Default Value<br></p> | 1:1          | 0     | 1            | Random                     | 100    | 100     |
| <p>Range<br></p>         | any          | 0–100 | .25 .5, or 1 | whole numbers 0–4294967295 | 10–100 | 0–1000  |

* Aspect ratios greater than 2:1 are experimental and may produce unpredicatble results.

### Model Version Parameters <a href="#model-version-parameters" id="model-version-parameters"></a>

Midjourney routinely releases new model versions to improve efficiency, coherency, and quality. Different models excel at different types of images.

#### Niji

`--niji` An alternative model focused on anime style images.

#### High Definition

`--hd` Use an early alternative Model that produces larger, less consistent images. This algorithm may be suitable for abstract and landscape images.

#### Test

`--test` Use the Midjourney special test model.

#### Testp

`--testp` Use the Midjourney special photography-focused test model.

#### Version

`--version <1, 2, 3, 4, or 5>` or `--v <1, 2, 3, 4, or 5>` Use a different version of the Midjourney algorithm. The current algorithm (V4) is the default setting.

### Upscaler Parameters <a href="#upscaler-parameters" id="upscaler-parameters"></a>

Midjourney starts by generating a grid of low-resolution image options for each Job. You can use a Midjourney upscaler on any grid image to increase the size and add additional details. There are multiple upscale models available for upscaling an image.

#### Uplight

`--uplight` Use an alternative "light" upscaler when selecting the U buttons. The results are closer to the original grid image. The upscaled image is less detailed and smoother.

#### Upbeta

`--upbeta` Use an alternative beta upscaler when selecting the U buttons. The results are closer to the original grid image. The upscaled image has significantly fewer added details.

#### Upanime

Use an alternative upscaler trained to work with the when selecting the U buttons. This upscaler was specifically created to work with the `--niji` Midjourney Model.

### Other Parameters <a href="#other-parameters" id="other-parameters"></a>

These parameters only work with specific earlier Midjourney Models

#### Creative

`--creative` Modify the `test` and `testp` models to be more varied and creative.

#### Image Weight

`--iw` Sets image prompt weight relative to text weight. The default value is --iw 0.25.

#### Sameseed

`--sameseed` Seed values create a single large random noise field applied across all images in the initial grid. When --sameseed is specified, all images in the initial grid use the same starting noise and will produce very similar generated images.

#### Video

`--video` Saves a progress video of the initial image grid being generated. Emoji react to the completed image grid with ✉️ to trigger the video being sent to your direct messages. `--video` does not work when upscaling an image.



### Compatibility <a href="#compatibility" id="compatibility"></a>

#### Model Version & Parameter Compatability

|                       | Affects initial generation | Affects variations + remix | Version 5                    | Version 4                    | Version 3                         | Test / Testp                      | Niji       |
| --------------------- | -------------------------- | -------------------------- | ---------------------------- | ---------------------------- | --------------------------------- | --------------------------------- | ---------- |
| Max Aspect Ratio      | ✓                          | ✓                          | any                          | 1:2 or 2:1                   | 5:2 or 2:5                        | 3:2 or 2:3                        | 1:2 or 2:1 |
| Chaos                 | ✓                          |                            | ✓                            | ✓                            | ✓                                 | ✓                                 | ✓          |
| Image Weight          | ✓                          |                            | <p>.5–2<br>default=1</p>     |                              | <p>any<br>default=.25</p>         | ✓                                 |            |
| No                    | ✓                          | ✓                          | ✓                            | ✓                            | ✓                                 | ✓                                 | ✓          |
| Quality               | ✓                          |                            | ✓                            | ✓                            | ✓                                 |                                   | ✓          |
| Seed                  | ✓                          |                            | ✓                            | ✓                            | ✓                                 | ✓                                 | ✓          |
| Sameseed              | ✓                          |                            |                              |                              | ✓                                 |                                   |            |
| Stop                  | ✓                          | ✓                          | ✓                            | ✓                            | ✓                                 | ✓                                 | ✓          |
| Style                 |                            |                            |                              | 4a and 4b                    |                                   |                                   |            |
| Stylize               | ✓                          |                            | <p>0–1000<br>default=100</p> | <p>0–1000<br>default=100</p> | <p>625–60000<br>default=2500)</p> | <p>1250–5000<br>default=2500)</p> |            |
| Tile                  | ✓                          | ✓                          | ✓                            |                              | ✓                                 |                                   |            |
| Video                 | ✓                          |                            |                              |                              | ✓                                 |                                   |            |
| Number of Grid Images | -                          | -                          | 4                            | 4                            | 4                                 | 2 (1 when aspect ratio≠1:1)       |            |



#### Deprecated Parameters

\--width and --w (replaced with --aspect)\
\--height and --h (replaced with --aspect)\
\--fast (replaced with --quality)\
\--vibe (now known as V1)\
\--hq\
\--newclip\
\--nostretch\
\--old\
\--beta
