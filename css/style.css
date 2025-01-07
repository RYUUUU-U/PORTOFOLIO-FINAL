// --- 
const tombolMenuHam = document.querySelector('.header__main-ham-menu-cont');
const menuKecil = document.querySelector('.header__sm-menu');
const tombolMenuHamHeader = document.querySelector('.header__main-ham-menu');
const tombolTutupMenuHamHeader = document.querySelector('.header__main-ham-menu-close');
const tautanMenuKecilHeader = document.querySelectorAll('.header__sm-menu-link');

tombolMenuHam.addEventListener('click', () => {
  if (menuKecil.classList.contains('header__sm-menu--active')) {
    menuKecil.classList.remove('header__sm-menu--active');
  } else {
    menuKecil.classList.add('header__sm-menu--active');
  }
  if (tombolMenuHamHeader.classList.contains('d-none')) {
    tombolMenuHamHeader.classList.remove('d-none');
    tombolTutupMenuHamHeader.classList.add('d-none');
  } else {
    tombolMenuHamHeader.classList.add('d-none');
    tombolTutupMenuHamHeader.classList.remove('d-none');
  }
});

for (let i = 0; i < tautanMenuKecilHeader.length; i++) {
  tautanMenuKecilHeader[i].addEventListener('click', () => {
    menuKecil.classList.remove('header__sm-menu--active');
    tombolMenuHamHeader.classList.remove('d-none');
    tombolTutupMenuHamHeader.classList.add('d-none');
  });
}

// --- 
const kontainerLogoHeader = document.querySelector('.header__logo-container');

kontainerLogoHeader.addEventListener('click', () => {
  location.href = 'index.html';
});

// --- Filter Projects and Certificates ---
const filterButtons = document.querySelectorAll('.filter-btn');
const projects = document.querySelectorAll('.projects__row');

filterButtons.forEach(button => {
  button.addEventListener('click', () => {
    const filter = button.getAttribute('data-filter');

    projects.forEach(project => {
      if (filter === 'all') {
        project.style.display = 'flex'; // Menampilkan semua proyek
      } else if (filter === '1-5') {
        const category = project.getAttribute('data-category');
        if (category >= 1 && category <= 5) {
          project.style.display = 'flex'; // Menampilkan proyek 1-5
        } else {
          project.style.display = 'none'; // Menyembunyikan proyek lainnya
        }
      } else if (filter === 'sololearn') {
        if (project.getAttribute('data-category') === 'sololearn') {
          project.style.display = 'flex'; // Menampilkan sertifikat SoloLearn
        } else {
          project.style.display = 'none'; // Menyembunyikan proyek lainnya
        }
      }
    });
  });
});
