FROM tensorflow/tensorflow:latest-gpu-jupyter

WORKDIR /app

COPY requirements.txt .
 
RUN pip install -r requirements.txt
  
EXPOSE 80                                           
ENTRYPOINT ["jupyter", "notebook", "--no-browser","--ip=0.0.0.0","--port=80","--NotebookApp.token=''","--NotebookApp.password=''"]
