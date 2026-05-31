const specialtyData = {
  nursing: {
    icon: 'heart-pulse',
    kicker: 'Специальность',
    title: 'Сестринское дело',
    text: 'Программа формирует профессиональные навыки ухода, коммуникации с пациентом, профилактики, сестринского процесса и работы в междисциплинарной команде.',
    list: ['Практика в клинических отделениях и симуляционном центре', 'Навыки пациентской безопасности и медицинской этики', 'Карьерный трек: медицинская сестра, старшая медсестра, координатор ухода']
  },
  medicine: {
    icon: 'stethoscope',
    kicker: 'Специальность',
    title: 'Лечебное дело',
    text: 'Подготовка специалистов первичного звена с акцентом на диагностику состояний, неотложную помощь, профилактику и маршрутизацию пациента.',
    list: ['Клиническое мышление и работа с протоколами', 'Навыки доврачебной и неотложной помощи', 'Практика в поликлиниках, стационарах и службах скорой помощи']
  },
  midwifery: {
    icon: 'baby',
    kicker: 'Специальность',
    title: 'Акушерское дело',
    text: 'Программа для будущих специалистов по сопровождению беременности, родовспоможению, уходу за матерью и ребёнком.',
    list: ['Практические занятия по акушерским алгоритмам', 'Профилактика осложнений и консультирование семей', 'Практика в женских консультациях и родильных отделениях']
  },
  pharmacy: {
    icon: 'pill',
    kicker: 'Специальность',
    title: 'Фармация',
    text: 'Обучение работе с лекарственными средствами, фармакологической информацией, аптечной практикой и безопасностью отпуска препаратов.',
    list: ['Фармакология и технология лекарственных форм', 'Навыки консультирования и контроля качества', 'Карьерный трек: аптечные сети, склады, фарморганизации']
  },
  dentistry: {
    icon: 'badge-plus',
    kicker: 'Специальность',
    title: 'Стоматология',
    text: 'Подготовка к работе в стоматологической практике с фокусом на ассистирование, профилактику, стерилизацию и коммуникацию с пациентом.',
    list: ['Ассистирование врачу-стоматологу', 'Инфекционный контроль и подготовка кабинета', 'Профилактические программы и обучение пациентов']
  },
  lab: {
    icon: 'microscope',
    kicker: 'Специальность',
    title: 'Лабораторная диагностика',
    text: 'Программа развивает компетенции в сборе, подготовке и анализе биоматериалов, лабораторной безопасности и интерпретации результатов.',
    list: ['Клиническая биохимия, микробиология и гематология', 'Стандарты лабораторной безопасности', 'Работа с современным аналитическим оборудованием']
  },
  optics: {
    icon: 'glasses',
    kicker: 'Специальность',
    title: 'Медицинская оптика',
    text: 'Направление готовит специалистов по подбору оптических средств коррекции зрения, консультированию и работе с оптическим оборудованием.',
    list: ['Основы анатомии и физиологии зрения', 'Подбор очковых линз и оптических изделий', 'Практика в оптиках и кабинетах коррекции зрения']
  },
  bachelor: {
    icon: 'graduation-cap',
    kicker: 'Программа',
    title: 'Прикладной бакалавриат',
    text: 'Расширенная практико-ориентированная программа для развития клинической самостоятельности, управления качеством ухода и лидерских компетенций.',
    list: ['Углублённая клиническая практика', 'Проектная работа и доказательная медицина', 'Подготовка к роли специалиста с расширенной ответственностью']
  }
};

const newsData = {
  simulation: {
    icon: 'activity',
    kicker: 'Новость · 15 мая 2026',
    title: 'Открытый день симуляционного обучения',
    text: 'На базе симуляционного центра прошёл практический день для студентов младших и старших курсов. Участники отработали сценарии первой помощи, сердечно-лёгочной реанимации и командного взаимодействия.',
    list: ['Сценарии неотложной помощи', 'Оценка навыков по чек-листам', 'Наставничество преподавателей-практиков']
  },
  grant: {
    icon: 'award',
    kicker: 'Новость · 27 апреля 2026',
    title: 'Консультации по грантам и поступлению',
    text: 'Приёмная комиссия запустила консультационные встречи для выпускников школ и родителей. На встречах объясняют условия конкурса, перечень документов и особенности выбора специальности.',
    list: ['Индивидуальный маршрут поступления', 'Проверка пакета документов', 'Разъяснение грантовых возможностей']
  },
  lab: {
    icon: 'microscope',
    kicker: 'Новость · 8 апреля 2026',
    title: 'Обновление лаборатории диагностики',
    text: 'Учебные лаборатории получили новое оснащение для практических занятий по клинической диагностике. Обновление помогает приблизить учебные задания к реальным рабочим процессам.',
    list: ['Новые лабораторные станции', 'Практические кейсы', 'Стандарты биологической безопасности']
  },
  career: {
    icon: 'handshake',
    kicker: 'Новость · 19 марта 2026',
    title: 'Карьерная неделя КВМК',
    text: 'Медицинские организации региона представили вакансии, требования к молодым специалистам и траектории профессионального роста для выпускников колледжа.',
    list: ['Встречи с работодателями', 'Разбор резюме и собеседований', 'Стажировки и практика']
  },
  volunteer: {
    icon: 'users-round',
    kicker: 'Новость · 4 марта 2026',
    title: 'Волонтёрская акция по профилактике',
    text: 'Студенты провели профилактическую акцию, посвящённую здоровому образу жизни, измерению базовых показателей и информированию населения.',
    list: ['Командная работа студентов', 'Коммуникация с населением', 'Профилактическая медицина']
  },
  conference: {
    icon: 'presentation',
    kicker: 'Новость · 21 февраля 2026',
    title: 'Студенческая научная конференция',
    text: 'На конференции были представлены проекты по качеству сестринского ухода, профилактике заболеваний, лабораторной диагностике и цифровым инструментам обучения.',
    list: ['Проектное мышление', 'Публичные выступления', 'Научные постеры и исследования']
  }
};

const body = document.body;
const mobileMenu = document.getElementById('mobileMenu');
const menuOpen = document.getElementById('menuOpen');
const menuClose = document.getElementById('menuClose');

function refreshIcons() {
  if (window.lucide) {
    window.lucide.createIcons();
  }
}

function openMenu() {
  mobileMenu.classList.remove('hidden');
  mobileMenu.setAttribute('aria-hidden', 'false');
  body.classList.add('menu-open');
  refreshIcons();
}

function closeMenu() {
  mobileMenu.classList.add('hidden');
  mobileMenu.setAttribute('aria-hidden', 'true');
  body.classList.remove('menu-open');
}

menuOpen?.addEventListener('click', openMenu);
menuClose?.addEventListener('click', closeMenu);
document.querySelectorAll('.mobile-link').forEach((link) => link.addEventListener('click', closeMenu));
mobileMenu?.addEventListener('click', (event) => {
  if (event.target === mobileMenu) closeMenu();
});

const modal = document.getElementById('contentModal');
const modalIcon = document.getElementById('modalIcon');
const modalKicker = document.getElementById('modalKicker');
const modalTitle = document.getElementById('modalTitle');
const modalText = document.getElementById('modalText');
const modalList = document.getElementById('modalList');

function setModalContent(data) {
  modalIcon.innerHTML = `<i data-lucide="${data.icon || 'sparkles'}"></i>`;
  modalKicker.textContent = data.kicker || 'КВМК';
  modalTitle.textContent = data.title || '';
  modalText.textContent = data.text || '';
  modalList.innerHTML = (data.list || [])
    .map((item) => `
      <div class="modal-list-item">
        <i data-lucide="check-circle-2"></i>
        <span>${item}</span>
      </div>
    `)
    .join('');
}

function openModal(data) {
  setModalContent(data);
  modal.classList.add('is-open');
  modal.setAttribute('aria-hidden', 'false');
  body.classList.add('modal-open');
  refreshIcons();
}

function closeModal() {
  modal.classList.remove('is-open');
  modal.setAttribute('aria-hidden', 'true');
  body.classList.remove('modal-open');
}

document.querySelectorAll('[data-specialty]').forEach((button) => {
  button.addEventListener('click', () => {
    const key = button.getAttribute('data-specialty');
    openModal(specialtyData[key]);
  });
});

document.querySelectorAll('[data-news]').forEach((card) => {
  card.addEventListener('click', () => {
    const key = card.getAttribute('data-news');
    openModal(newsData[key]);
  });
  card.tabIndex = 0;
  card.setAttribute('role', 'button');
  card.addEventListener('keydown', (event) => {
    if (event.key === 'Enter' || event.key === ' ') {
      event.preventDefault();
      const key = card.getAttribute('data-news');
      openModal(newsData[key]);
    }
  });
});

document.querySelectorAll('[data-close-modal]').forEach((button) => button.addEventListener('click', closeModal));
modal?.addEventListener('click', (event) => {
  if (event.target === modal) closeModal();
});

const lightbox = document.getElementById('lightbox');
const lightboxImage = document.getElementById('lightboxImage');
const lightboxClose = document.getElementById('lightboxClose');

function openLightbox(src) {
  lightboxImage.src = src;
  lightbox.classList.add('is-open');
  lightbox.setAttribute('aria-hidden', 'false');
  body.classList.add('modal-open');
}

function closeLightbox() {
  lightbox.classList.remove('is-open');
  lightbox.setAttribute('aria-hidden', 'true');
  lightboxImage.src = '';
  body.classList.remove('modal-open');
}

document.querySelectorAll('[data-lightbox]').forEach((button) => {
  button.addEventListener('click', () => openLightbox(button.getAttribute('data-lightbox')));
});
lightboxClose?.addEventListener('click', closeLightbox);
lightbox?.addEventListener('click', (event) => {
  if (event.target === lightbox) closeLightbox();
});

document.addEventListener('keydown', (event) => {
  if (event.key === 'Escape') {
    closeModal();
    closeLightbox();
    closeMenu();
  }
});

const revealElements = document.querySelectorAll('.reveal');
const revealObserver = new IntersectionObserver((entries) => {
  entries.forEach((entry) => {
    if (entry.isIntersecting) {
      entry.target.classList.add('is-visible');
      revealObserver.unobserve(entry.target);
    }
  });
}, { threshold: 0.14 });

revealElements.forEach((element) => revealObserver.observe(element));

const stats = document.querySelectorAll('[data-count]');
let statsStarted = false;

function easeOutCubic(value) {
  return 1 - Math.pow(1 - value, 3);
}

function animateNumber(element, target, suffix) {
  const duration = 1700;
  const start = performance.now();
  const formatter = new Intl.NumberFormat('ru-RU');

  function frame(now) {
    const progress = Math.min((now - start) / duration, 1);
    const value = Math.floor(easeOutCubic(progress) * target);
    element.textContent = `${formatter.format(value)}${suffix}`;
    if (progress < 1) requestAnimationFrame(frame);
  }

  requestAnimationFrame(frame);
}

const statsObserver = new IntersectionObserver((entries) => {
  if (statsStarted) return;
  const visible = entries.some((entry) => entry.isIntersecting);
  if (!visible) return;
  statsStarted = true;
  stats.forEach((element) => {
    animateNumber(element, Number(element.dataset.count), element.dataset.suffix || '');
  });
}, { threshold: 0.25 });

const statsSection = document.querySelector('[aria-labelledby="stats-title"]');
if (statsSection) statsObserver.observe(statsSection);

const contactForm = document.getElementById('contactForm');
const toast = document.getElementById('toast');
let toastTimer;

contactForm?.addEventListener('submit', (event) => {
  event.preventDefault();
  contactForm.reset();
  toast.classList.add('is-visible');
  clearTimeout(toastTimer);
  toastTimer = setTimeout(() => toast.classList.remove('is-visible'), 4200);
  refreshIcons();
});

refreshIcons();
