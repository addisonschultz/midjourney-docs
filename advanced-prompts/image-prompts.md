# Image Prompts

**You can use images as part of a prompt to influence a Job's composition, style, and colors. Images prompts can be used alone or with text prompts—experiment with combining images with different styles for the most exciting results.**

To add images to a prompt, type or paste the web address where the image is stored online. The address must end in an extension like .png, .gif, or .jpg. After adding image addresses, add any additional text and parameters to complete the prompt.

![Image showing the Midjourney prompt structure.](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ%20Prompt.png)

Image prompts go at the front of a prompt.\
Prompts must have two images or one image and additional text to work.\
An image URL must be a direct link to an online image.\
In most browsers, right-click or long-press an image and select Copy Image Address to get the URL.\
The `/blend` command is a simplified image prompting process optimized for mobile users.

***

### Upload an image to Discord <a href="#upload-an-image-to-discord" id="upload-an-image-to-discord"></a>

To use a personal image as part of a prompt, upload it to Discord. To upload an image, click the **Plus** sign next to where messages are typed. Select **Upload a File**, select an image, and send the message. To add this image to a prompt, begin typing `/imagine` as usual. After the prompt box appears, drag the image file into the prompt box to add the image's URL. Alternatively, right-click the image, select **Copy Link**, and then paste the link within the prompt box.

![Discord\_FHZfwDLhLY.gif](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/Discord\_FHZfwDLhLY.gif)

Privacy Notes

Upload images in your Direct Messages with the Midjourney Bot to prevent other server users from seeing an image.\
Image prompts are visible on the Midjourney website unless a user has Stealth Mode.

***

### Examples <a href="#examples" id="examples"></a>

#### Starting Images

![Cropped image of the Bust of Apollo](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ\_ImagePrompt\_Statue.png)

Statue of Apollo

![Cropped image of vintage flower illustraiton](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ\_ImagePrompt\_Flowers.png)

Vintage Flower Illustration

![Cropped image of Ernst Haeckel's Jellyfish](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ\_ImagePrompt\_Jelly.jpg)

Ernst Haeckel's Jellyfish

![Cropped image of Ernst Haeckel's Lichen](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ\_ImagePrompt\_Lichen.png)

Ernst Haeckel's Lichen

![Cropped image of The Great Wave off Kanagawa](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ\_ImagePrompt\_Wave.png)

Hokusai's The Great Wave

#### Midjourney Model Version 4

***

#### Midjourney Model Version 5

Aspect Ratio Tip

Crop images to the same aspect ratio as your final image for the best results.

***

### Image Weight Parameter <a href="#image-weight-parameter" id="image-weight-parameter"></a>

Use the image weight parameter `--iw` to adjust the importance of the image vs. text portion of a prompt. The default value is used when no `--iw` is specified. Higher `--iw` values mean the image prompt will have more impact on the finished job.

See the Multi Prompts page for more information about the relative importance between parts of a prompt.

Different Midjourney Version Models have different image weight ranges.

|                 | Version 5 | Version 4 | Version 3    | Test / Testp | niji |
| --------------- | --------- | --------- | ------------ | ------------ | ---- |
| Stylize default | 1         | NA        | .25          | NA           | NA   |
| Stylize Range   | .5–2      | NA        | -10000–10000 | NA           | NA   |

prompt example: `/imagine prompt` `flowers.jpg birthday cake --iw .5`

![Cropped image of painter Jan Davidsz. de Heem's Vase of Flowers used a midjourney image prompt](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/mj\_iw-start.jpg)

Image Prompt

![A midjourney image generated from the prompt, a birthday cake with the image weight parameter set to .5](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/mj\_iw-0-50.png)

\--iw .5

![A midjourney image generated from the prompt, a birthday cake with the image weight parameter set to .75](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/mj\_iw-0-75.png)

\--iw .75

![A midjourney image generated from the prompt, a birthday cake with the image weight parameter set to 1.5](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/mj\_iw-1-00.png)

\--iw 1

![A midjourney image generated from the prompt, a birthday cake with the image weight parameter set to 0](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/mj\_iw-1-25.png)

\--iw 1.25

![A midjourney image generated from the prompt, a birthday cake with the image weight parameter set to 1.5](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/mj\_iw-1-50.png)

\--iw 1.5

![A midjourney image generated from the prompt, a birthday cake with the image weight parameter set to 1.75](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/mj\_iw-1-75.png)

\--iw 1.75

![A midjourney image generated from the prompt, a birthday cake with the image weight parameter set to 2](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/mj\_iw-2-00.png)

\--iw 2

Subscribers can work one-on-one with the Midjourney Bot in Discord's Direct Messages instead of a public channel. Images made within your direct messages are still subject to content and moderation rules and will be visible on your Midjourney website gallery.
