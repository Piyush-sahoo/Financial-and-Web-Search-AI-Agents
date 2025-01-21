\documentclass{article}
\usepackage{hyperref}
\usepackage{listings}
\usepackage{xcolor}
\usepackage{enumitem}
\usepackage{geometry}

\geometry{margin=1in}

\definecolor{codegreen}{rgb}{0,0.6,0}
\definecolor{codegray}{rgb}{0.5,0.5,0.5}
\definecolor{backcolour}{rgb}{0.95,0.95,0.92}

\lstdefinestyle{mystyle}{
    backgroundcolor=\color{backcolour},   
    commentstyle=\color{codegreen},
    basicstyle=\ttfamily\small,
    breakatwhitespace=false,         
    breaklines=true,                 
    keepspaces=true,                 
    showspaces=false,                
    showstringspaces=false,
    showtabs=false,                  
    tabsize=2
}

\lstset{style=mystyle}

\begin{document}

\title{Financial and Web Search AI Agents}
\author{}
\date{}

\maketitle

\section*{Overview}
This project showcases the integration of advanced AI agents designed for financial analysis and web search functionalities. It uses the \texttt{phi} framework to create specialized agents capable of leveraging tools like YFinance and DuckDuckGo to provide users with actionable insights.

\section{Main Components}
This repository contains two main agents:
\begin{itemize}
    \item \textbf{Web Search Agent}: Designed to perform web searches and fetch information using DuckDuckGo.
    \item \textbf{Finance AI Agent}: Provides financial insights such as stock prices, analyst recommendations, company news, and stock fundamentals using YFinance.
\end{itemize}

Both agents are designed to interact seamlessly and provide results in an intuitive format like tables, with a strong emphasis on user-friendly outputs.

\section{Features}

\subsection{Financial Data Analysis}
\begin{itemize}
    \item Fetch stock prices, analyst recommendations, and financial fundamentals
    \item Summarize the latest company news
\end{itemize}

\subsection{Web Search}
\begin{itemize}
    \item Search the web for information with source citations
\end{itemize}

\subsection{Multi-agent Collaboration}
\begin{itemize}
    \item Combine agents for comprehensive outputs
\end{itemize}

\subsection{Interactive Playground}
\begin{itemize}
    \item Host and interact with agents via a user-friendly FastAPI playground
\end{itemize}

\section{Installation}

\subsection{Clone the Repository}
\begin{lstlisting}[language=bash]
git clone https://github.com/your-repo-name.git
cd your-repo-name
\end{lstlisting}

\subsection{Install Dependencies}
\begin{lstlisting}[language=bash]
pip install -r requirements.txt
\end{lstlisting}

\subsection{Environment Setup}
Create a \texttt{.env} file in the root directory with:
\begin{lstlisting}
OPENAI_API_KEY=your_openai_api_key
PHI_API_KEY=your_phi_api_key
\end{lstlisting}

\section{Usage}

\subsection{Running the Financial Agent}
Execute predefined queries:
\begin{lstlisting}[language=bash]
python financial_agent.py
\end{lstlisting}

\subsection{Launching the Playground}
Start the interactive playground:
\begin{lstlisting}[language=bash]
python playground.py
\end{lstlisting}
Access the playground at \url{http://127.0.0.1:8000}

\section{Agents}

\subsection{Web Search Agent}
\begin{itemize}
    \item \textbf{Role}: Fetches web information
    \item \textbf{Tools}: DuckDuckGo
    \item \textbf{Features}:
    \begin{itemize}
        \item Includes source citations
        \item Outputs results in markdown format
    \end{itemize}
\end{itemize}

\subsection{Finance AI Agent}
\begin{itemize}
    \item \textbf{Role}: Performs financial analysis
    \item \textbf{Tools}: YFinance
    \item \textbf{Features}:
    \begin{itemize}
        \item Displays financial data in tables
        \item Fetches stock prices, fundamentals, recommendations, and news
    \end{itemize}
\end{itemize}

\section{Environment Variables}
Required environment variables in \texttt{.env} file:
\begin{itemize}
    \item \texttt{OPENAI\_API\_KEY}: API key for OpenAI integration
    \item \texttt{PHI\_API\_KEY}: API key for the Phi framework
\end{itemize}

\section{Dependencies}
Main Python packages:
\begin{itemize}
    \item \texttt{phidata}: Core framework for building AI agents
    \item \texttt{python-dotenv}: For loading environment variables
    \item \texttt{yfinance}: Fetching financial data
    \item \texttt{duckduckgo-search}: Web search functionality
    \item \texttt{fastapi} and \texttt{uvicorn}: Hosting the interactive playground
    \item \texttt{groq}: Model integration for advanced AI capabilities
    \item \texttt{openai}: OpenAI API integration
\end{itemize}

Install dependencies:
\begin{lstlisting}[language=bash]
pip install -r requirements.txt
\end{lstlisting}

\section{Contributing}
Contributions are welcome! Please fork the repository and submit a pull request with your proposed changes.

\section{License}
This project is licensed under the MIT License. See the LICENSE file for details.

\end{document}
