FROM mcr.microsoft.com/playwright
WORKDIR /app
COPY requirements.txt /
USER pwuser
ENV PATH="/home/pwuser/.local/bin:${PATH}"
RUN python3 -m pip install --user --upgrade pip
RUN python3 -m pip install --user -r /requirements.txt
CMD python init.py