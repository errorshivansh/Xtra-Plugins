# Xtra-Plugins - TezerUB ✨
> A Repo That Contains Many X-Tra Plugins From TezerDevs And Third Parties.

# Example 👊

### Plugins 🔧

```python3
from main_startup.core.decorators import Tezer_on_cmd
from main_startup.helper_func.basic_helpers import edit_or_reply

@Tezer_on_cmd(['helloworld'],
    cmd_help={
    "help": "This is A TEST",
    "example": "{ch}helloworld"
    })
async def hello_world(client, message):
    mg = await edit_or_reply(message, "`Hello World! This Works!`")
```
### Custom Filters 📣

```python3
from main_startup.core.decorators import listen

@listen(filters.mentioned & ~filters.me)
async def mentioned_(client, message):
    await message.reply_text("`Hello World! Btw Why Did You Mention Me?`")
```

# Credit 💝
* Friday 
* Userge
* Userge X
