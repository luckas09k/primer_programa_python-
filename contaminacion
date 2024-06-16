import discord
from discord.ext import commands
import os
import random

intents = discord.Intents.default()
intents.message_content = True

bot = commands.Bot(command_prefix='?', intents=intents)

@bot.event
async def on_ready():
    print(f"¡Hola!, Soy el Bot de la Descontaminación y te enseñaré que es la Contaminacion y como prevenirla ")

@bot.command()
async def Contaminacion(ctx):
    await ctx.send(f"La contaminación es la presencia de un constituyente, impureza o algún otro elemento indeseable que estropea, corrompe, infecta, inutiliza o degrada un material, cuerpo físico, entorno natural, lugar de trabajo, etc. La contaminación ambiental o polución es la introducción de sustancias nocivas u otros elementos físicos en un medio ambiente, que provocan que este sea inseguro o no apto para su uso. El medio ambiente puede ser un ecosistema, un medio físico o un ser vivo. El contaminante puede ser una sustancia química o energía (como sonido, calor, luz o radiactividad). Es siempre una alteración negativa del estado natural del medio ambiente y, por lo general, se produce como consecuencia de la actividad humana considerándose una forma de impacto ambiental.")

@bot.command()
async def Como_prevenirlo(ctx):
    await ctx.send(f"Aqui hay algunas imagenes que te enseñarán a prevenir la contaminación")
    lista = os.listdir("Imagenes_anticontaminacion")
    anticontaminacion_random = random.choice(lista)
    with open(f'Imagenes_anticontaminacion/{anticontaminacion_random}', 'rb') as f:
        picture = discord.File(f)
    f.close
    await ctx.send(file=picture)


bot.run("MTI0Njg1NzM5MzIxMjQ4OTgxOQ.GhAuSu.YdcCkrd5ItzbqKvOLBZRzir3fdZUDra29VQcxU")
