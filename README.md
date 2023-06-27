# Python Dataset for Four of Mark Watson's Books

Text from books:

- LangChain and LlamaIndex Projects Lab Book: Hooking Large Language Models Up to the Real World
- Loving Common Lisp, or the Savvy Programmer's Secret Weapon
- Haskell Tutorial and Cookbook
- Practical Artificial Intelligence Programming With Java

## License

You are free to:

Share — copy and redistribute the material in any medium or format

Adapt — remix, transform, and build upon the material for any purpose, even commercially.

Under the following terms:

Attribution — You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.

ShareAlike — If you remix, transform, or build upon the material, you must distribute your contributions under the same license as the original.

## How you can add attribution

You can reference my name and the Leanpub web page for my eBooks:

    https://leanpub.com/u/markwatson

## Use with the Python datasets libray

Install the library:

    pip install datasets

Interactive example:

```
$ python
Python 3.10.8 (main, Nov 24 2022, 08:08:27) [Clang 14.0.6 ] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> from datasets import load_dataset
>>> ds = load_dataset(path="mark_watson_books")
Downloading and preparing dataset text/mark_watson_books to /Users/markwatson/.cache/huggingface/datasets/text/mark_watson_books-938bf857e5e87466/0.0.0/cb1e9bd71a82ad27976be3b12b407850fe2837d80c22c5e03a28949843a8ace2...
Downloading data files: 100%|█████████████████████████████████████████████████████████████████| 1/1 [00:00<00:00, 8338.58it/s]
Extracting data files: 100%|███████████████████████████████████████████████████████████████████| 1/1 [00:00<00:00, 311.64it/s]
Dataset text downloaded and prepared to /Users/markwatson/.cache/huggingface/datasets/text/mark_watson_books-912bf857e5e87466/0.0.0/cb1e9bd71a82ad27976be3b12b407850fe2837d80c22c5e03a28949843a8ace2. Subsequent calls will reuse this data.
100%|██████████████████████████████████████████████████████████████████████████████████████████| 1/1 [00:00<00:00, 397.15it/s]
>>> ds
DatasetDict({
    train: Dataset({
        features: ['text'],
        num_rows: 23809
    })
})
>>> text = ds['train']['text']
>>> text
>>> text
['Haskell Tutorial and Cookbook', 'Mark Watson', ...
```
