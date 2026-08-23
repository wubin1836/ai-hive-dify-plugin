# AI Hive AIGC Models for Dify

AI Hive AIGC Models brings commercial image and video generation into Dify through one provider credential. It is built for e-commerce operators, designers, marketing and advertising teams, brands, content creators, short-drama teams, and AI workflow builders.

[Chinese documentation](README.zh_Hans.md)

## Tools

- **Generate or Edit Image** with Nano Banana Pro, GPT Image 2, Seedream 5 Lite, Nano Banana 2, and other image models available to the connected AI Hive account.
- **Generate or Edit Video** with Seedance, MiniMax H3, HappyHorse, and other video models available to the connected AI Hive account. Supported workflows depend on the selected model and can include text-to-video, image-to-video, reference-to-video, video editing, and extension.
- **Query Generation Task** to continue checking a submitted task without submitting it again.

## Typical use cases

- Product hero images, listing galleries, product detail pages, posters, ad creative, retouching, and background replacement.
- Product demonstrations, shoppable videos, UGC-style ads, TV commercials, social video, short drama, and animated comics.
- Content production for Amazon, TikTok Shop, Shopify, Shopee, Lazada, Temu, AliExpress, SHEIN, Instagram, and major Chinese e-commerce platforms.

## Installation and configuration

1. Install the plugin from Dify Marketplace or from a local `.difypkg` file.
2. Create an AI Hive API key in the AI Hive API access panel.
3. Open the AI Hive provider authorization panel in Dify.
4. Paste the API key beginning with `sk-api-` and save the credential.
5. Add one of the three AI Hive tools to a Dify Agent, Workflow, or Chatflow.

## Usage example

For an e-commerce image workflow, select **Generate or Edit Image**, choose a model such as Nano Banana Pro or GPT Image 2, enter the product-image prompt, and optionally attach reference images. For video, select **Generate or Edit Video**, choose an available Seedance or MiniMax model, enter the prompt, and attach the model-supported reference media.

The plugin reads live model metadata and pricing snapshots before each submission. Long-running tasks can be checked again with **Query Generation Task**.

## Connection requirements

- Outbound HTTPS access to `https://ai-hive.iclip.cn/api`.
- A valid AI Hive API key.
- Network access to model result URLs returned by AI Hive.

AI Hive is an external service. Model usage may consume paid AI Hive credits according to the pricing shown in the user's AI Hive account; the Dify plugin itself does not sell a subscription or process payments.

The plugin sends prompts, generation parameters, and user-supplied reference media to AI Hive only when required to complete the requested task. It does not embed or log the user's API key.

## Development

```bash
python3 -m unittest discover -s tests -v
dify plugin package ./ai-hive-dify-plugin
```

Source repository: <https://github.com/wubin1836/ai-hive-dify-plugin>

## Trademark notice

Model names, platform names, and company names are used only to describe compatibility and production intent. This plugin does not claim an official partnership with those third parties.

## License

MIT
