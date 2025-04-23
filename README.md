<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
</head>
<body>
  <h1>👀 Sistema de Monitoramento com Detecção de Pessoas</h1>

  <p>Projeto em Python que utiliza <strong>YOLOv8</strong> para detectar pessoas em tempo real a partir de uma <strong>câmera IP via RTSP</strong>. Ideal para monitorar ambientes como a cozinha e enviar alertas quando alguém for detectado.</p>

  <p><strong>Motivação:</strong> Desenvolvi esse sistema para conseguir estudar e trabalhar com mais tranquilidade, evitando que meu filho, entre na cozinha sozinho e faça alguma arte enquanto eu tô concentrado.</p>

  <h2>🚀 Funcionalidades</h2>
  <ul>
    <li>🎥 Acesso ao stream da câmera IP via protocolo RTSP</li>
    <li>🧠 Detecção de pessoas usando o modelo <strong>YOLOv8</strong></li>
    <li>✅ Tratamento de IP dinâmico da câmera</li>
    <li>🧒 <em>(Em desenvolvimento)</em> Reconhecimento facial para detectar apenas o Miguel</li>
  </ul>

  <h2>🛠 Tecnologias Utilizadas</h2>
  <ul>
    <li>Python 3.12+</li>
    <li><a href="https://github.com/ultralytics/ultralytics" target="_blank">Ultralytics YOLOv8</a></li>
    <li>OpenCV</li>
    <li>NumPy</li>
  </ul>

  <h2>🖼 Exemplo de uso</h2>
  <pre><code>python monitoramento.py</code></pre>

  <p>A aplicação conecta ao RTSP da câmera e inicia a detecção de pessoas em tempo real. Ao identificar uma pessoa no quadro, uma caixa delimitadora será desenhada com a label "person".</p>
 <h2>📷 Resultado</h2>
<p>Exemplo real de detecção na prática :</p>
<img src="midia/miguxo após sair.jpg" alt="Detecção de pessoa com YOLOv8" width="400"/>
  <h2>⚙ Configuração</h2>
  <ol>
    <li>Instale as dependências:
      <pre><code>pip install -r requirements.txt</code></pre>
    </li>
    <li>Configure a URL RTSP da sua câmera:
      <pre><code>rtsp_url = "rtsp://usuario:senha@ip_da_camera:554/onvif1"</code></pre>
    </li>
  </ol>
  <p>⚠ Certifique-se de que a câmera está na mesma rede e com o IP atualizado.</p>

  <h2>📦 Estrutura do Projeto</h2>
  <pre><code>📁 projeto-monitoramento
├── monitoramento.py        # Código principal
├── requirements.txt        # Dependências
├── dados/foto.png          # Foto para aparecer ao ser detectado
└── README.md               # Este arquivo</code></pre>

  <h2>📋 To-do</h2>
  <ul>
    <li>✅ Detecção de pessoas com YOLOv8</li>
    <li>✅ Conexão com câmera IP (RTSP)</li>
    <li>✅ Tratamento de IP dinâmico</li>
    <li>⬜ Reconhecimento facial básico</li>
    <li>⬜ Interface gráfica (GUI)</li>
  </ul>

  <hr>

</body>
</html>
