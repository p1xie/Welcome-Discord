# Welcome-Discord

const Discord = require("discord.js");
const client = new Discord.Client();

client.on('ready', () => {
  console.log(`Logged in as ${client.user.username}#${client.user.discriminator}`);
});

client.on('message', msg => {
  if (msg.content === 'ping') msg.reply('Pong!');
});

client.login('some cool token');
      
