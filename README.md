# LangChain 練習：打造 SequentialChain 應用

## 使用 Colab 前的準備

| 變數名稱            | 用途                         | 設定範例（請改成自己的金鑰）     |
|---------------------|------------------------------|----------------------------------|
| `OPENAI_API_KEY`    | OpenAI 服務呼叫憑證          | `export OPENAI_API_KEY="sk-..."` |
| `GOOGLE_API_KEY`    | Google Generative AI 金鑰    | `export GOOGLE_API_KEY="..."`    |
| `GOOGLE_CSE_ID`     | Google Custom Search Engine | `export GOOGLE_CSE_ID="..."`     |

> 建議在 Colab 的 **啟動程式碼區塊**（或使用 `secrets`）中先行設定，避免憑證洩漏。

## 安裝套件

在 Colab 的第一個程式碼區塊執行以下指令，一口氣完成所有依賴安裝與升級：

```bash
!pip install -U \
    openai \
    langchain \
    langchain-openai \
    langchain-community \
    langchain-google-genai \
    --quiet

