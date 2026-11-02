
1. Create and activate a virtual environment:

   ```bash
   uv venv
   source .venv/bin/activate
   ```

2. Install the required Python packages using the following command:
   ```bash
   pip install -r requirements.txt
   ``` 

3. Run the RBC Explorer script to start exploring and downloading documents from RBC websites:

   ```bash
   python -m chatbot.rag.rbc_explorer
    Success! 18 documents have been downloaded to the 'rbc_documents' folder.
    You can now run your RAG chatbot with these documents.
   ```

4. Save RBC Investment FAQs:

   ```bash
   python -m chatbot.rag.save_investment_faqs
   ```
   Webpage content saved to ./rbc_documents/rbc_investment_faqs.txt
   RBC Investment FAQs have been successfully saved.


5. Run the MCP server with SSE support:
```bash
uv run --no-project --python .venv/bin/python python -m chatbot.mcp.server_sse

Added to Python path: /Users/garychew/Documents/Galileo/llm-chatbot
/Users/garychew/Documents/Galileo/llm-chatbot/chatbot/rag/rag_chatbot.py:4: FutureWarning: 

All support for the `google.generativeai` package has ended. It will no longer be receiving 
updates or bug fixes. Please switch to the `google.genai` package as soon as possible.
See README for more details:

https://github.com/google-gemini/deprecated-generative-ai-python/blob/main/README.md

import google.generativeai as genai
Database bank.db already initialized.
Vector store not found. Creating new vector store...
Loaded 88 pages from irdeck2026q3.pdf
Loaded 40 pages from PDA_Account_Disclosure_Booklet.pdf
fontTools is required to fully parse the encoding of a CFF Type1 font in font dictionary {'/BaseFont': '/HUHTVJ+RBCText-Regular', '/Encoding': IndirectObject(71, 0, 4681538192), '/FirstChar': 9, '/FontDescriptor': IndirectObject(73, 0, 4681538192), '/LastChar': 31, '/Subtype': '/Type1', '/Type': '/Font', '/Widths': [650, 576, 659, 533, 370, 603, 749, 608, 288, 654, 603, 288, 556, 534, 574, 406, 726, 647, 713, 497, 510, 603, 898]}, but is not installed. Consider installing fontTools if you encounter encoding problems.
Loaded 2 pages from what_you_need_to_open_an_account_or_cash_certain_government_of_canada_cheques.pdf
Loaded 4 pages from quick-reference-guide.pdf
fontTools is required to fully parse the encoding of a CFF Type1 font in font dictionary {'/BaseFont': '/CCIKLX+RBCText-Regular', '/Encoding': IndirectObject(615, 0, 4681346112), '/FirstChar': 14, '/FontDescriptor': IndirectObject(616, 0, 4681346112), '/LastChar': 31, '/Subtype': '/Type1', '/Type': '/Font', '/Widths': [528, 611, 749, 533, 603, 370, 574, 510, 603, 330, 659, 726, 647, 713, 497, 598, 620, 898]}, but is not installed. Consider installing fontTools if you encounter encoding problems.
Loaded 2 pages from Startup%20costs%20template.pdf
Loaded 10 pages from br-value-program.pdf
Loaded 9 pages from linked-loyalty-terms-en.pdf
Loaded 120 pages from 2026englishproxy.pdf
Loaded 1 pages from Payrol-Direct-Deposit-EN.pdf
fontTools is required to fully parse the encoding of a CFF Type1 font in font dictionary {'/BaseFont': '/JSDXAP+RBCText-Regular', '/Encoding': IndirectObject(1294, 0, 4677743184), '/FirstChar': 11, '/FontDescriptor': IndirectObject(1296, 0, 4677743184), '/LastChar': 31, '/Subtype': '/Type1', '/Type': '/Font', '/Widths': [650, 576, 659, 533, 603, 749, 370, 330, 603, 288, 556, 534, 574, 406, 726, 647, 713, 497, 510, 603, 898]}, but is not installed. Consider installing fontTools if you encounter encoding problems.
Loaded 36 pages from mca-agreement-en.pdf
Loaded 3 pages from newsletters-rbc-investment-update.pdf
Loaded 5 pages from Terms-and-Conditions.pdf
Loaded 2 pages from newsletters-rbc-select-portfolios.pdf
```


