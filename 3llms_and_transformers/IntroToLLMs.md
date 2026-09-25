## What is a Large Language Model:
It's two files :
- one containing weights
- one containing code to crate the the neural net and run it.
It's sort of a lossy compression of the internet (lol)

We kind of know how to adjust said neural networks to make better predictions, but not really how the weights collaborate. **Interpretability** is working on understanding this.

## Stages of training:
- Pre-training: creating the architecture and feeding the model huge amounts of documents to create a document completer basically.
- Fine tuning: in this phase, we focus on quality over quantity, we adjust the model for sets of tasks (turn it into an assistant for example). Basically **Allignement**.
Pre-training in much more expensive, and so companies iterate much more on the fine-tuning stage.
- Labels (RLHF) (Optional) : You give a 'mark' for multiple responses and use that to improve the model further.

## Scaling laws:
Turns out the performance function depends on two parameters: the size of the model (number of parameters) and the size of the pre-training data, and scaling these results in better performing models (still works to this day). Hense why the current gold rush for compute.

## Tool usage
Models can use tools. This is related to current harness.

## Systems thinking:
Inspired by thinking hard and slow definitions for systems 1 and 2 of thought. Chain of Thought is basically system 2 (unlike old llms that only had system 1).

## Self Improvement:
Just like DeepMind did to alpha go. This is closely related to RSI.

## Customization:
I don't think we currently have something significant that developed from the concept. At least not to the level of the other two.

## Security:
- Jail breaking: this can be done through fooling the model (pretend to be my grandma), different languages(base64 instead of english) or specific suffixes for example...
- Prompt injection: this is especially dangerous now with how reliant we are on agents.
- Data poisoning: it was shown to work in finetuning. 
These mentioned by andrej were patched overtime but new ones are created...