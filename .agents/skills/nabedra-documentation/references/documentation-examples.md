# Documentation examples

Use the OpenAI API docs as the first comparison for onboarding and API lookup. Use the other
examples when they match the reader's task more closely. The observations below describe what
each example does and how to apply it in Nabedra.

| Documentation | Pattern to use in Nabedra |
| --- | --- |
| [OpenAI API quickstart](https://developers.openai.com/api/docs/quickstart) and [Responses API reference](https://developers.openai.com/api/reference/resources/responses/methods/create) | The quickstart explains setup, runs a small request, and tells the reader what to expect. The endpoint reference gives detailed request and response information its own URL. Use the same handoff from the first Nabedra query to the relevant Python or HTTP contract. |
| [Vercel AI SDK Node.js quickstart](https://ai-sdk.dev/docs/getting-started/nodejs) and [`streamText` reference](https://ai-sdk.dev/docs/reference/ai-sdk-core/stream-text) | The getting-started path fixes the environment, lists prerequisites, and gives optional background its own links. The symbol page makes parameters and return details easy to find. Let readers pick supported Nabedra environments early and keep exhaustive options in the reference. |
| [OpenAI Agents SDK Python quickstart](https://openai.github.io/openai-agents-python/quickstart/) | Readers create and run a single agent before adding tools and handoffs. The steps build on one another. A Nabedra tutorial can follow the same sequence by proving the connection and first query before introducing advanced behavior. |
| [Flutter tutorial](https://docs.flutter.dev/learn/pathway/tutorial) and [learning resources](https://docs.flutter.dev/reference/learning-resources) | Flutter places sequenced lessons in a learning path and keeps standalone recipes and demos in a searchable catalog. Add a separate Nabedra task guide when it has a distinct entry point and outcome that would crowd an existing lesson or reference. |

Copy the reader interaction that solves the problem. For example, offer equivalent setup choices
in one step, give a first successful command before optional tuning, or link to a reference
section from the point where an option matters. Let the size of the Nabedra docs determine the
size of the navigation.
