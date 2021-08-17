# tickets

import telebot

bot = telebot.TeleBot('1967870742:AAFhuXnzw2-ik2dvWn5kIxk2WH3RDaDfSAM')
@bot.message_handler(commands=['start'])
def start_command(message):
    bot.send_message(message.chat.id, "Hello!")
bot.polling()
