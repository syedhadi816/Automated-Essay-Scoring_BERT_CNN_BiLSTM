# A Context Aware Neural Network for Prompt Independent Automated Essay Scoring 

One of the primary concerns in AES is the lack of portability across different domains and
prompts. Most existing AES systems are trained on specific essay prompts, making it difficult
to apply the same model to evaluate essays written in response to different prompts or subject
matters. This limitation has led to the development of models that can better adapt to new
contexts and essay types, thus improving their utility and applicability in various educational
environments.
In this study, we investigate the performance of two AES models—a classification model and
a regression model—by leveraging state-of-the-art natural language processing techniques,
including the use of BERT embeddings for essays. BERT provides the model with a more
context-aware vector representation than traditional techniques such as word2vec, resulting in
improved performance in capturing the nuances of written text. Although many attempts have
been made to utilize pretrained models like BERT in AES, they have yet to consistently
outperform other deep learning models, such as LSTM. The classification model, which
categorizes essays into two classes (good and bad), provides a weak learning mechanism that
can potentially aid transfer learning for cross-prompt essay scoring. By using a simplified
representation of essay quality, the classification model may be more adaptable to different
prompts and domains, as it focuses on general features of good and bad essays, rather than
attempting to predict precise scores.
In this paper, we propose an approach that combines deep learning models with pretrained
models. Specifically, we employ BERT embeddings as input to a neural network architecture
that includes a convolutional neural network (CNN) for sentence embeddings and a
bidirectional long short-term memory (Bi-LSTM) for essay embeddings. This combination of
pretrained and deep learning models aims to take advantage of the strengths of both approaches, 
potentially leading to improved performance in AES tasks.
