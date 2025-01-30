# README for Colab Notebook

## 1. Setting Up ngrok
To enable external access to the Colab notebook, you need to use ngrok. Follow these steps:

1. Visit the [ngrok website](https://ngrok.com/) and create an account if you don’t have one.
2. Once logged in, go to the **Dashboard** and find your **ngrok authentication token**.
3. Copy the token and paste it into the Colab notebook when prompted to set up ngrok.

**Note:** Without the ngrok token, the notebook will not establish the required external tunnel.

---

## 2. Loading the vLLM Model
The notebook uses the `deepseek-ai/DeepSeek-R1-Distill-Qwen-1.5B` model, which is loaded using vLLM. Please note:

1. **Initial Loading Time:** The first time the model is initialized, it will take some time to download and load the model into memory. This is normal and expected.

2. **Manual Restart Required:** Once the model is fully loaded, the Jupyter cell may still appear to be running. In this case:
    - Interrupt the execution of the cell.
    - Restart the cell to ensure the model is ready to be used.

**Important:** Do not attempt to use the model before restarting the cell after the initial load, as it may not function correctly.

---

By following these instructions, you can ensure the smooth operation of the Colab notebook.
