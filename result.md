# Parameter Experiment Results

## Prompt: Item: A bow crafted by elves

| Temperature | Output |
|-------------|--------|
| 0.7         | Predictable and basic bow description |
| 1.0         | More creative language and details |
| 1.5         | Weird and sometimes nonsense text, but imaginative |

## Prompt: Quest: Rescue the princess from

| Seed | Output |
|------|--------|
| 42   | Dragon-related quest |
| 100  | Orc tribe scenario |
| None | Random each time |

## Learnings

- Temperature controls randomness: higher = more creative, lower = more accurate.
- Seed gives reproducibility.

## Next Steps

- Add a web API using Flask
- Fine-tune on a fantasy game dataset
