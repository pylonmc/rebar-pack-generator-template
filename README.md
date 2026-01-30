# 🎨 Rebar Resource Pack Generator

This repo contains a resourcepack generator for [Rebar]() addons.
If you are an addon developer that wants to create a resource pack for your addon, or you're just someone unaffiliated who wants to make a resource pack for an addon, this generator may be of use to you!

## Rebar Resource Pack Support

Rebar offers lots of tools and systems for addons to enable using resource packs to further elevate gameplay.
This pack generator makes it easier to take advantage of those tools, most importantly, custom block textures.

## Why Use It?

Because Rebar supports **not** using resource packs, all of the systems have to be optional, which makes actually using the systems more complicated.
Whenever you want to add a model to a pylon item, you have to add an entry to the *vanilla* item model which backs that pylon item. 
As you add models for more and more items, the more large, complicated, and messy, the item models will get, and if an addon makes breaking changes, it becomes even trickier to update.

This is especially true for custom block models, Rebar supports custom block textures by *using item models*, which means there is no actual block state system.
In order to use rebar block states, you have to manually handle a LOT of custom model data, which exponentially increases the more properties a block has. Manually creating the item model definition entries for even a block such as a lever, becomes a **monumental** task for the normal person. This pack generator enables you to use the vanilla block state format and will automatically create ALL of the item models and item model definitions needed for the block.

If you think you're up for the task of using block states for custom block models with Rebar without using a pack generator, [here](./assets/example_custom_lever.json)'s an example of what you need to create a lever with all of the vanilla block states.

# Usage

Refer to the [Wiki]() for detailed instructions on how you can use the pack generator!