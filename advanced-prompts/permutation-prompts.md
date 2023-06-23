# 📟 Permutation Prompts

**Permutation Prompts allow you to quickly generate variations of a Prompt with a single `/imagine` command. By including lists of options separated with commas `,` within curly braces `{}` in your prompt, you can create multiple versions of a prompt with different combinations of those options.**

You can use Permutation Prompts to create combinations and permutations involving any part of a Midjourney Prompt, including text, image prompts, parameters, or prompt weights.

Permutation prompts are only available for Pro Subscribers using Fast mode.

***

### Permutation Prompt Basics <a href="#permutation-prompt-basics" id="permutation-prompt-basics"></a>

Separate your list of options within curly brackets {} to quickly create and process multiple prompt variations.

**Prompt Example:**\
`/imagine prompt` `a {red, green, yellow} bird` creates and processes three Jobs.

`/imagine prompt` `a red bird`\
`/imagine prompt` `a green bird`\
`/imagine prompt` `a yellow bird`

GPU Minutes

The Midjourney Bot processes each Permutation Prompt variation as an individual Job, each Job consumes GPU minutes.

Combo Prompts that create more than five Jobs will show a confirmation message before they begin processing.

***

### Permutation Prompt Examples <a href="#permutation-prompt-examples" id="permutation-prompt-examples"></a>

#### Prompt Text Variations

The prompt `/imagine prompt` `a naturalist illustration of a {pineapple, blueberry, rambutan, banana} bird` will create and process four Jobs:

![A midjourney generated image of a a pineapple bird](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ\_Combo\_pineappleBird.jpg)

a naturalist illustration of a pineapple bird

![A midjourney generated image of a blueberry bird](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ\_Combo\_blueberryBird.jpg)

a naturalist illustration of a blueberry bird

![A midjourney generated image of a rambutan bird](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ\_Combo\_rambutanBird.jpg)

a naturalist illustration of a rambutan bird

![A midjourney generated image of a banana bird](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ\_Combo\_bananaBird.jpg)

a naturalist illustration of a banana bird

***

#### Prompt Parameter Variations

The prompt `/imagine prompt` `a naturalist illustration of a fruit salad bird --ar {3:2, 1:1, 2:3, 1:2}` will create and process four Jobs with different aspect ratios:

![A midjourney generated image of a fruit salad bird with a 3:2 aspect ratio](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ\_combo\_AR32.jpg)

a naturalist illustration of a fruit salad bird --ar 3:2

![A midjourney generated image of a fruit salad bird with a 1:1 aspect ratio](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ\_combo\_AR11.png)

a naturalist illustration of a fruit salad bird --ar 1:1

![A midjourney generated image of a fruit salad bird with a 2:3 aspect ratio](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ\_combo\_AR23.jpg)

a naturalist illustration of a fruit salad bird --ar 2:3

![A midjourney generated image of a fruit salad bird with a 1:1 aspect ratio](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ\_combo\_AR12.jpg)

a naturalist illustration of a fruit salad bird --ar 1:2

The prompt `/imagine prompt` `a naturalist illustration of a fruit salad bird --{v 5, niji, test}` will create and process three Jobs using different Midjourney Model Versions:

![A midjourney generated image of a fruit salad bird using the v5 model](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ\_Combo\_v5.jpg)

a naturalist illustration of a fruit salad bird --v 5

![A midjourney generated image of a fruit salad bird using the niji model](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ\_Combo\_niji.jpg)

a naturalist illustration of a fruit salad bird --niji

![A midjourney generated image of a fruit salad bird using the test model](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ\_Combo\_test.jpg)

a naturalist illustration of a fruit salad bird --test

***

#### Multiple and Nested Permutations

It is possible to use multiple sets of bracketed options in a single prompt.\
`/imagine prompt` `a {red, green} bird in the {jungle, desert}` creates and processes four Jobs.

`/imagine prompt` `a red bird in the jungle`\
`/imagine prompt` `a red bird in the desert`\
`/imagine prompt` `a green bird in the jungle`\
`/imagine prompt` `a green bird in the desert`

It is also possible to nest sets of bracketed options inside other sets of brackets within a single prompt:

Example: `/imagine prompt` `A {sculpture, painting} of a {seagull {on a pier, on a beach}, poodle {on a sofa, in a truck}}.`

`/imagine prompt` `A sculpture of a seagull on a pier.`\
`/imagine prompt` `A sculpture of a seagull on a beach.`\
`/imagine prompt` `A sculpture of a poodle on a sofa.`\
`/imagine prompt` `A sculpture of a poodle in a truck.`\
`/imagine prompt` `A painting of a seagull on a pier.`\
`/imagine prompt` `A painting of a seagull on a beach.`\
`/imagine prompt` `A painting of a poodle on a sofa.`\
`/imagine prompt` `A painting of a poodle in a truck.`

***

#### Escape Character

If you want to include a `,` within the curly brackets that does not act as a separator place a backslash `\` directly before it.

`imagine prompt` `{red, pastel, yellow} bird` produces three Jobs\
`/imagine prompt` `a red bird`\
`/imagine prompt` `a pastel bird`\
`/imagine prompt` `a yellow bird`

`imagine prompt` `{red, pastel \, yellow} bird` produces two Jobs\
`/imagine prompt` `a red bird`\
`/imagine prompt` `a pastel, yellow bird`

A maximum of 40 Jobs can be created with a single Permutation Prompt.

A Prompt is a short text phrase that the Midjourney Bot interprets to produce an image. The Midjourney Bot breaks down the words and phrases in a prompt into smaller pieces, called tokens, that can be compared to its training data and then used to generate an image. A well-crafted prompt can help make unique and exciting images.

There are two modes for image generation, **Fast Mode** and **Relax Mode**. Fast Mode tries to give you a GPU instantly. It's the highest-priority processing tier and uses your subscription's monthly GPU time. **Relax Mode** queues your generation behind others based on how much you've used the system. **Relax Mode** wait times are variable and usually range from 1–10 minutes.

By default, your images will be generated using **Fast** mode. You can switch to **Relax** if you have a Standard or Pro subscription.

A **Job** is any action that uses the Midjourney Bot. **Jobs** include using `/imagine` to create an initial image grid, upscaling images, and creating variations of images.

The Midjourney Bot processes jobs on high-end GPUs. Each minute that it takes to complete a job is a **GPU minute**. You have a limited amount of GPU minutes when in **Fast Mode**. Because image generations may be processed on multiple GPUs simultaneously, GPU minutes are not directly connected to the time you wait for an image to generate.
