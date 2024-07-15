const moment = require('moment-timezone');

module.exports = {
  config: {
    name: "time",
    version: "0.1",
    author: "red wan",
    countdown: 5,
    role: 0,
    shortDescription: "Displays the current date and time of bangladesh.",
    longDescription: "",
    category: "misc",
    guide: "{prefix}{name}",
    envConfig: {}
  },

  onStart: async function({ message, args }) {
    const bangladeshTime = moment.tz("Asia/Bangladesh").format("h:mm:ss A");
    const bangladeshDate = moment.tz("Asia/Bangladesh").format("dddd, DD MMMM YYYY");

    const reply = `Today Date & Time in the Bangladesh:\n` +
      `❏Date: ${bangladeshDate}\n` +
      `❏Time: ${bangladeshTime}`;

    message.reply(reply);
  },
  onEvent: async function() {}
};
