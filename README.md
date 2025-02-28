# Guide to Increase Context Length for a Model in Ollama

This guide provides step-by-step instructions on how to increase the context length of a model downloaded from Ollama.

## Prerequisites

Before you begin, ensure that you have:

- Installed Ollama on your machine.
- Downloaded the model you want to work with.

## Steps to Increase Context Length

1. **Run the Model**

   First, run the model that you want to modify by executing the following command in your terminal:
   ```bash
   ollama run model_name
   ```

2. **Set the Context Length**

   Once the model is running, set the new context length by using the `/set` command. Replace `num_ctx` with the desired number of tokens for the context length:
   ```bash
   /set parameter num_ctx <desired_number>
   ```

3. **Save the Model**

   After adjusting the context length, save the modified model under a new name:
   ```bash
   /save new_model_name_you_want
   ```

4. **Hit Enter**

   Press `Enter` to confirm the changes and save the model with the updated context length.

5. **Verify the Changes**

   To verify that the context length has been updated successfully, list all your models by running:
   ```bash
   ollama list
   ```

   You should see your newly saved model in the list.

## Notes

- The context length (`num_ctx`) determines how much information the model can consider in a single request. Increasing this can improve the model’s ability to process longer inputs, but it may also impact performance.

## Conclusion

By following these steps, you should be able to successfully increase the context length of any model downloaded from Ollama. For more advanced configurations, refer to Ollama's official documentation.
