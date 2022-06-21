# Google Tag Manager template for Adless

This template allows you to start earning with Adless by serving your content without ads in no time!

The template is available from the [Community Template Gallery](https://tagmanager.google.com/gallery/#/?filter=adless).

See [adless.net/get-started/gtm](https://adless.net/get-started/gtm) for instructions on how to get started.

## Note: Tag Sequencing

This template is optimized for using tag sequencing to handle fallback behavior if the visitor does not pay for not seeing ads. The tag will behave as follows:

- If the visitor is authenticated with Adless and pays for not seeing ads, the tag will **fail**.
- Otherwise the tag will **succeed**.

The reason for this is that we want to use a cleanup trigger to run any fallback and GTM only allows you to condition cleanup on failures, not success. To do so, you need to use the "Don't fire <cleanup tag> if <this tag> fails" option as described in the [Tag Manager Help](https://support.google.com/tagmanager/answer/6238868). See [adless.net/get-started/gtm](https://adless.net/get-started/gtm) for further information. 