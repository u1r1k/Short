import os
from telegram import Update
from telegram.ext import Updater, CommandHandler, CallbackContext

TOKEN = os.getenv("6409245799:AAEMc3oHaZWuaVzIcHm2Gu2hlxp0rEJl8HM")  # Храним токен в переменных окружения
def start(update: Update, context: CallbackContext):
    update.message.reply_text("👋 Привет! Я бот, и я работаю на Render!")

def main():
    updater = Updater(token=TOKEN, use_context=True)
    dp = updater.dispatcher
    dp.add_handler(CommandHandler("start", start))

    print("🤖 Бот запущен")
    updater.start_polling()
    updater.idle()

if __name__ == "__main__":
    main()
