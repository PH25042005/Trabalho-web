const modal = document.getElementById('modal');
const modalImage = document.getElementById('modal-image');
const closeModalButton = document.getElementById('close-modal');
const openModalButtons = document.querySelectorAll('.open-modal');

openModalButtons.forEach(button => {
  button.addEventListener('click', () => {
    modalImage.src = button.dataset.img;
    modal.style.display = 'flex';
  });
});

closeModalButton.addEventListener('click', () => {
  modal.style.display = 'none';
});
