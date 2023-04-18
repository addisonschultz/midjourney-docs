# Seeds

**The Midjourney bot uses a seed number to create a field of visual noise, like television static, as a starting point to generate the initial image grids. Seed numbers are generated randomly for each image but can be specified with the `--seed` or `--sameseed` parameter. Using the same seed number and prompt will produce similar ending images.**

* `--seed` accepts whole numbers 0–4294967295.
* `--seed` values only influence the initial image grid.
* Identical `--seed` values using Model Versions `1`, `2`, `3`, `test`, and `testp` will produce images with similar composition, color, and details.
* Identical `--seed` values using Model Versions `4`, `5`, and `niji` will produce nearly identical images.
* Seed numbers are not static and should not be relied upon between sessions.

***

If no Seed is specified, Midjourney will use a randomly generated seed number, producing a wide variety of options each time a prompt is used.

#### Jobs run three times with random seeds:

prompt example: `/imagine prompt` `celadon owl pitcher`

\


#### Jobs run two times with `--seed 123`:

prompt example: `/imagine prompt` `celadon owl pitcher --seed 123`

![An example of an image grid made in midjourney V4 with a random seed](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ\_Seed-123\_V4\_.png)

![An example of an image grid made in midjourney V4 with a random seed](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ\_Seed-123\_V4\_.png)

***

### Sameseed Parameter <a href="#sameseed-parameter" id="sameseed-parameter"></a>

`--seed` values create a single large random noise field applied across all images in the initial grid. When `--sameseed` is specified, all images in the initial grid use the same starting noise and will produce very similar generated images.

`--sameseed` accepts whole numbers 0–4294967295.\
`--sameseed` is only compatible with Model Versions `1`, `2`, `3`, `test`, and `testp`.

**Early visual noise from**\
**`--sameseed`**

![Example image of early noise field used to generate images with Midjourney parameter sameseed](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ\_Sameseed\_Stop10.png)

`--sameseed 12345`

**Finished Job made with**\
**`--sameseed`**

![Example image images with Midjourney parameter sameseed](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ\_Sameseed.png)

`--sameseed 12345`

**Early visual noise without**\
**`--sameseed`**

![Example image of early noise field used to generate images with Midjourney](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ\_seed\_Stop10.png)

`--seed 12345`

**Finished Job made without**\
**`--sameseed`**

![Example image image made with Midjourney](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ\_seed.png)

`--seed 12345`

***

### How to Find a Job's Seed Number <a href="#how-to-find-a-job-s-seed-number" id="how-to-find-a-job-s-seed-number"></a>

#### Use a Discord Emoji Reaction

Find the seed number of a Job in discord by reacting with an ✉️ envelope emoji to a Job.

![Animated Gif showing how to use the Emoji React with an Envelope in Discord to find a Job's seed number](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ\_JobID\_EmojiReact.gif)

#### Use The Show Command to Bring Back Old Jobs

To get the seed number for a past image, copy the job ID and use the `/show <Job ID #>` command with that ID to revive the Job. You can then react to the newly regenerated Job with an ✉️ envelope emoji.

***

### How To Change Seed Numbers <a href="#how-to-change-seed-numbers" id="how-to-change-seed-numbers"></a>

#### Use the `--seed` or `--sameseed` Parameter

Add `--seed <value>` or `--sameseed <value>` to the end of your prompt.

![Animated Gif showing how the Midjourney Seed parameter is typed](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ\_Seed\_Gif.gif)

A **Job** is any action that uses the Midjourney Bot. **Jobs** include using `/imagine` to create an initial image grid, upscaling images, and creating variations of images.
