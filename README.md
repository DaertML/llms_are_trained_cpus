# llms_are_trained_cpus
Repository to experiment with LLMs as if they were CPUs by training and testing them with different embeddings.
More than a repository, I feel like the main place where things will happen in this repo, is the README.md, and
will likely use the rest of the repository to store the examples.

# Introduction:
LLMs (mainly Language Models that follow the Transformer architecture: either using the Encoder-Decoder, Encoder only,
or Decoder only architectures) behave in a similar way as a CPU in a computer works.

If we consider them as a black box; they receive an input, and produce an output. Digging a bit deeer, we find that
the input to the model is text in a natural language and output is text in a natural language as well (we are not
considering other kinds of inputs to transformers, just yet. In order to keep it simple and lay the ideas that refer
to the repository; somehow they can be extended to music and visual transformers, as well as transformers that receive
any other kind of input).

We can agree that such text in natural language is similar to high level programming languages like python, if we keep
the analogy that LLMs behave like CPUs. Because of that, if we dig further the natural text is translated into tokens
using the tokenizer; such tokens are integer ids, that represent the introduced text. Some tokenizers will create embeddings
from the input text mapping each text token to a numerical ID, others will map the input text to a different length embedding.

The tokens introduced into the LLM are the machine code, if we resemble the metaphor to how programming languages get to run
in a CPU. Because of that, code compiled for a certain CPU architecture, will not work in a different CPU architecture (ARM vs. x86);
in a similar manner, it is expected that the same happens for the LLM, unless...

And this is where this gets interesting; LLMs are not a 1 to 1 mapping (or metaphor) to CPUs, in this case LLMs are "trained" CPUs
in a way in which, the LLM will (likely) be capable of generating output for a given input in a embedding language (I am coining this
term as the way a natural text gets transformed into the input ids introduced in the LLM).
