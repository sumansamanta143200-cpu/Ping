const { bot } = require('../lib/')

bot(
  {
    pattern: 'ping ?(.*)',
    desc: 'To check ping',
    type: 'misc',
  },
  async (message, match) => {
    const start = new Date().getTime()
    await message.send('```𝐂𝐫𝐮𝐬𝐡 𝐂𝐚𝐦𝐞 𝐢𝐧 𝐅𝐫𝐨𝐧𝐭 𝐨𝐟 𝐌𝐞..!```')
    const end = new Date().getTime()
    return await message.send('*💗𝑯𝒆𝒂𝒓𝒕 𝑹𝒂𝒕𝒆..*\n ' + (end - start) + ' ʙᴘᴍ')
  }
)
