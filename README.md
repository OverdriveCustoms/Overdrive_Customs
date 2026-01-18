document.getElementById('year').textContent = new Date().getFullYear();

document.getElementById('contactForm').addEventListener('submit', function(e){
  e.preventDefault();
  const status = document.getElementById('formStatus');
  status.textContent = 'Enviando... (esto es solo una demo)';
  // Aquí podrías enviar el formulario a un servidor o a un servicio como Formspree.
  setTimeout(()=> {
    status.textContent = 'Mensaje enviado. ¡Gracias!';
    this.reset();
  }, 900);
});
