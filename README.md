from discord.ext import commands
import random

bot = commands.Bot(command_prefix='?')


@bot.command()
async def example(ctx):
    await ctx.send(f"{random.choice(ctx.guild.members).mention}")

bot.run('')
