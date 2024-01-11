///賢い使い方を知っている場合のみ使用すること。
@bot.event
async def on_ready():
    guild_count = len(bot.guilds)
    member_count = sum(len(guild.members) for guild in bot.guilds)

    status = disnake.Status.dnd
    activity = disnake.Activity(
        type=disnake.ActivityType.watching,
        name=f"{member_count} users!"
    )

    await bot.change_presence(status=status, activity=activity)

    print(f"bot name: {bot.user.name}")
    print(f"guild count: {guild_count}")
    print(f"membercount: {member_count}")

@bot.event
async def on_member_join(member):
    member_count = sum(len(guild.members) for guild in bot.guilds)
    activity = disnake.Activity(
        type=disnake.ActivityType.watching,
        name=f"{member_count} users!"
    )
    await bot.change_presence(activity=activity)

@bot.event
async def on_member_remove(member):
    member_count = sum(len(guild.members) for guild in bot.guilds)
    activity = disnake.Activity(
        type=disnake.ActivityType.watching,
        name=f"{member_count} users!"
    )
    await bot.change_presence(activity=activity)
/// 賢い使い方を知っている場合のみ使用すること。
