# inssanmartin.github.io
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Instituto San Martín | Excelencia Educativa desde 1985</title>
    
    <!-- Meta tags mejorados para SEO -->
    <meta name="description" content="Instituto San Martín: Formación integral de líderes desde 1985. Programas de Primaria, Secundaria y Bachillerato. Excelencia académica con valores sólidos.">
    <meta name="robots" content="index, follow">
    <meta name="author" content="Instituto San Martín">
    <meta name="keywords" content="educación, escuela, instituto, primaria, secundaria, bachillerato, formación, líderes">
    
    <link rel="canonical" href="https://www.institutosanmartin.edu/">
    <link rel="icon" href="data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'><text y='.9em' font-size='90'>📚</text></svg>">

    <!-- Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet">
    
    <style>
        /* === VARIABLES CSS === */
        :root {
            --primary: #ea580c;
            --primary-dark: #c2410c;
            --primary-light: #fed7aa;
            --secondary: #1e40af;
            --dark: #111827;
            --light: #f9fafb;
            --gray: #6b7280;
            --gray-light: #e5e7eb;
            --white: #ffffff;
            --shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            --shadow-lg: 0 10px 25px rgba(0, 0, 0, 0.15);
            --radius: 8px;
            --radius-lg: 12px;
            --transition: all 0.3s ease;
            --font-heading: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
            --font-body: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
        }

        /* === ESTILOS PERSONALIZADOS MANTENIDOS === */
        html {
            scroll-behavior: smooth;
            scroll-padding-top: 80px;
        }

        body {
            font-family: var(--font-body);
            line-height: 1.6;
            color: #333;
            overflow-x: hidden;
        }

        /* Tipografía personalizada */
        h1, h2, h3, h4 {
            font-family: var(--font-heading);
            font-weight: 700;
            line-height: 1.2;
            margin-bottom: 1rem;
            color: var(--dark);
        }

        h1 {
            font-size: clamp(2.5rem, 5vw, 3.5rem);
        }

        h2 {
            font-size: clamp(2rem, 4vw, 2.5rem);
            position: relative;
            padding-bottom: 0.5rem;
        }

        h2::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 60px;
            height: 4px;
            background: var(--primary);
            border-radius: 2px;
        }

        h2.text-center::after {
            left: 50%;
            transform: translateX(-50%);
        }

        h3 {
            font-size: clamp(1.5rem, 3vw, 1.75rem);
        }

        .lead {
            font-size: 1.25rem;
            font-weight: 300;
        }

        /* Secciones */
        .section {
            padding: 5rem 0;
            position: relative;
        }

        .section-bg {
            background-color: var(--light);
        }

        .section-accent {
            background: linear-gradient(135deg, var(--primary) 0%, var(--primary-dark) 100%);
            color: var(--white);
        }

        /* Tarjetas personalizadas */
        .custom-card {
            background: var(--white);
            border-radius: var(--radius-lg);
            overflow: hidden;
            transition: var(--transition);
            height: 100%;
            display: flex;
            flex-direction: column;
            cursor: pointer;
            position: relative;
            border: none;
            box-shadow: var(--shadow);
        }

        .custom-card:hover {
            transform: translateY(-5px);
            box-shadow: var(--shadow-lg);
        }

        .custom-card-img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .custom-card-content {
            padding: 1.5rem;
            flex-grow: 1;
            display: flex;
            flex-direction: column;
        }

        .card-icon {
            width: 64px;
            height: 64px;
            background: var(--primary-light);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 1rem;
            color: var(--primary);
        }

        .card-icon-sm {
            width: 48px;
            height: 48px;
            background: var(--primary-light);
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 1rem;
            color: var(--primary);
        }

        /* Estadísticas */
        .stat-item {
            text-align: center;
            padding: 1.5rem;
            background: var(--white);
            border-radius: var(--radius-lg);
            box-shadow: var(--shadow);
            transition: var(--transition);
        }

        .stat-item:hover {
            transform: translateY(-3px);
        }

        .stat-number {
            font-size: 2.5rem;
            font-weight: 700;
            color: var(--primary);
            margin-bottom: 0.5rem;
        }

        /* Testimonios */
        .testimonial-card {
            background: rgba(255, 255, 255, 0.1);
            border: 1px solid rgba(255, 255, 255, 0.2);
            border-radius: var(--radius-lg);
            padding: 2rem;
            height: 100%;
            display: flex;
            flex-direction: column;
        }

        .quote-icon {
            color: var(--primary-light);
            margin-bottom: 1rem;
            font-size: 2rem;
        }

        .testimonial-text {
            flex-grow: 1;
            font-style: italic;
            margin-bottom: 1.5rem;
            color: var(--white);
            opacity: 0.95;
        }

        /* Formulario de contacto personalizado */
        .custom-form label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 500;
            color: var(--dark);
        }

        .custom-form input,
        .custom-form textarea,
        .custom-form select {
            width: 100%;
            padding: 0.875rem 1rem;
            border: 2px solid var(--gray-light);
            border-radius: var(--radius);
            font-size: 1rem;
            font-family: inherit;
            transition: var(--transition);
        }

        .custom-form input:focus,
        .custom-form textarea:focus,
        .custom-form select:focus {
            outline: none;
            border-color: var(--primary);
            box-shadow: 0 0 0 3px rgba(234, 88, 12, 0.1);
        }

        .custom-form textarea {
            min-height: 150px;
            resize: vertical;
        }

        /* Mapa */
        .map-container {
            border-radius: var(--radius-lg);
            overflow: hidden;
            height: 300px;
            margin-top: 2rem;
        }

        /* Footer personalizado */
        .footer {
            background: var(--dark);
            color: var(--white);
            padding: 4rem 0 2rem;
        }

        .footer-brand {
            display: flex;
            align-items: center;
            gap: 0.75rem;
            font-size: 1.25rem;
            font-weight: 700;
            margin-bottom: 1rem;
            color: var(--white);
        }

        .footer-links {
            list-style: none;
            padding-left: 0;
        }

        .footer-links li {
            margin-bottom: 0.75rem;
        }

        .footer-links a {
            color: rgba(255, 255, 255, 0.7);
            text-decoration: none;
            transition: var(--transition);
        }

        .footer-links a:hover {
            color: var(--white);
        }

        .social-links {
            display: flex;
            gap: 1rem;
            margin-top: 1rem;
        }

        .social-link {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background: rgba(255, 255, 255, 0.1);
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--white);
            text-decoration: none;
            transition: var(--transition);
        }

        .social-link:hover {
            background: var(--primary);
        }

        .footer-bottom {
            padding-top: 2rem;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            text-align: center;
            color: rgba(255, 255, 255, 0.6);
        }

        /* Modales personalizados */
        .custom-modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: rgba(0, 0, 0, 0.8);
            z-index: 3000;
            overflow-y: auto;
            padding: 2rem;
        }

        .custom-modal.active {
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .custom-modal-content {
            background: var(--white);
            border-radius: var(--radius-lg);
            max-width: 800px;
            width: 100%;
            max-height: 90vh;
            overflow-y: auto;
            position: relative;
        }

        /* Hero Section personalizada */
        .hero {
            height: 100vh;
            min-height: 700px;
            background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), 
                        url('https://images.unsplash.com/photo-1626402570254-3e3d1790e14f?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&q=80&w=1920') center/cover no-repeat;
            color: var(--white);
            padding: 2rem 1rem;
        }

        .hero-content {
            max-width: 800px;
            margin: 0 auto;
            position: relative;
            z-index: 2;
        }

        .hero h1 {
            color: var(--white);
            margin-bottom: 1.5rem;
        }

        .hero-subtitle {
            font-size: 1.5rem;
            margin-bottom: 2.5rem;
            opacity: 0.9;
        }

        /* Botones personalizados */
        .btn-custom-primary {
            background: var(--primary);
            color: var(--white);
            border: none;
            padding: 0.75rem 1.5rem;
            border-radius: var(--radius);
            font-weight: 600;
            transition: var(--transition);
        }

        .btn-custom-primary:hover {
            background: var(--primary-dark);
            transform: translateY(-2px);
            box-shadow: var(--shadow-lg);
            color: var(--white);
        }

        .btn-custom-outline {
            background: transparent;
            color: var(--white);
            border: 2px solid var(--white);
            padding: 0.75rem 1.5rem;
            border-radius: var(--radius);
            font-weight: 600;
            transition: var(--transition);
        }

        .btn-custom-outline:hover {
            background: var(--white);
            color: var(--primary);
        }

        /* Iconos */
        .icon-container {
            width: 48px;
            height: 48px;
            background: var(--primary-light);
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-shrink: 0;
            color: var(--primary);
        }

        /* Responsive adjustments */
        @media (max-width: 768px) {
            .section {
                padding: 3rem 0;
            }

            .hero {
                min-height: 600px;
                padding: 1rem;
            }

            .hero h1 {
                font-size: 2.5rem;
            }

            .hero-subtitle {
                font-size: 1.25rem;
            }
        }

        @media (max-width: 480px) {
            .hero h1 {
                font-size: 2rem;
            }
        }

        /* Utilitarios */
        .text-primary { color: var(--primary) !important; }
        .text-white { color: var(--white) !important; }
        .text-primary-light { color: var(--primary-light) !important; }
        .cursor-pointer { cursor: pointer; }
        
        /* Estilos para política de privacidad */
        .privacy-content {
            font-size: 0.95rem;
            line-height: 1.7;
        }
        
        .privacy-content h2, 
        .privacy-content h3 {
            color: var(--dark);
            margin-top: 1.5rem;
            margin-bottom: 0.75rem;
        }
        
        .privacy-content ul {
            padding-left: 1.5rem;
            margin-bottom: 1rem;
        }
        
        .privacy-content li {
            margin-bottom: 0.5rem;
        }
        
        .privacy-content strong {
            color: var(--dark);
        }
    </style>
</head>
<body>
    <!-- Modal de Política de Privacidad (ACTUALIZADO) -->
    <div id="privacyPolicyModal" class="custom-modal">
        <div class="custom-modal-content">
            <button class="btn-close position-absolute top-0 end-0 m-3" onclick="closeModal('privacyPolicyModal')"></button>
            <div class="p-4 privacy-content">
                <h1 class="text-primary mb-4">POLÍTICA DE PRIVACIDAD DEL SITIO WEB</h1>
                
                <h2>I. POLÍTICA DE PRIVACIDAD Y PROTECCIÓN DE DATOS</h2>
                <p>Respetando lo establecido en la legislación vigente, Instituto San Martín (en adelante, también Sitio Web) se compromete a adoptar las medidas técnicas y organizativas necesarias, según el nivel de seguridad adecuado al riesgo de los datos recogidos.</p>
                
                <h3>Leyes que incorpora esta política de privacidad</h3>
                <p>Esta política de privacidad está adaptada a la normativa española y europea vigente en materia de protección de datos personales en internet. En concreto, la misma respeta las siguientes normas:</p>
                <ul>
                    <li>El Reglamento (UE) 2016/679 del Parlamento Europeo y del Consejo, de 27 de abril de 2016, relativo a la protección de las personas físicas en lo que respecta al tratamiento de datos personales y a la libre circulación de estos datos (RGPD).</li>
                    <li>La Ley Orgánica 3/2018, de 5 de diciembre, de Protección de Datos Personales y garantía de los derechos digitales (LOPD-GDD).</li>
                    <li>El Real Decreto 1720/2007, de 21 de diciembre, por el que se aprueba el Reglamento de desarrollo de la Ley Orgánica 15/1999, de 13 de diciembre, de Protección de Datos de Carácter Personal (RDLOPD).</li>
                    <li>La Ley 34/2002, de 11 de julio, de Servicios de la Sociedad de la Información y de Comercio Electrónico (LSSI-CE).</li>
                </ul>
                
                <h3>Identidad del responsable del tratamiento de los datos personales</h3>
                <p>El responsable del tratamiento de los datos personales recogidos en Instituto San Martín es: Gerard Durán López, con NIF: (en adelante, Responsable del tratamiento). Sus datos de contacto son los siguientes:</p>
                <ul>
                    <li><strong>Dirección:</strong> Calle Andalusia Nº12</li>
                    <li><strong>Teléfono de contacto:</strong> 640774704</li>
                    <li><strong>Email de contacto:</strong> milaloab240681@gmail.com</li>
                </ul>
                
                <h3>Registro de Datos de Carácter Personal</h3>
                <p>En cumplimiento de lo establecido en el RGPD y la LOPD-GDD, le informamos que los datos personales recabados por Instituto San Martín, mediante los formularios extendidos en sus páginas quedarán incorporados y serán tratados en nuestro fichero con el fin de poder facilitar, agilizar y cumplir los compromisos establecidos entre Instituto San Martín y el Usuario o el mantenimiento de la relación que se establezca en los formularios que este rellene, o para atender una solicitud o consulta del mismo.</p>
                <p>Asimismo, de conformidad con lo previsto en el RGPD y la LOPD-GDD, salvo que sea de aplicación la excepción prevista en el artículo 30.5 del RGPD, se mantiene un registro de actividades de tratamiento que especifica, según sus finalidades, las actividades de tratamiento llevadas a cabo y las demás circunstancias establecidas en el RGPD.</p>
                
                <h2>Principios aplicables al tratamiento de los datos personales</h2>
                <p>El tratamiento de los datos personales del Usuario se someterá a los siguientes principios recogidos en el artículo 5 del RGPD y en el artículo 4 y siguientes de la Ley Orgánica 3/2018, de 5 de diciembre, de Protección de Datos Personales y garantía de los derechos digitales:</p>
                <ul>
                    <li><strong>Principio de licitud, lealtad y transparencia:</strong> se requerirá en todo momento el consentimiento del Usuario previa información completamente transparente de los fines para los cuales se recogen los datos personales.</li>
                    <li><strong>Principio de limitación de la finalidad:</strong> los datos personales serán recogidos con fines determinados, explícitos y legítimos.</li>
                    <li><strong>Principio de minimización de datos:</strong> los datos personales recogidos serán únicamente los estrictamente necesarios en relación con los fines para los que son tratados.</li>
                    <li><strong>Principio de exactitud:</strong> los datos personales deben ser exactos y estar siempre actualizados.</li>
                    <li><strong>Principio de limitación del plazo de conservación:</strong> los datos personales solo serán mantenidos de forma que se permita la identificación del Usuario durante el tiempo necesario para los fines de su tratamiento.</li>
                    <li><strong>Principio de integridad y confidencialidad:</strong> los datos personales serán tratados de manera que se garantice su seguridad y confidencialidad.</li>
                    <li><strong>Principio de responsabilidad proactiva:</strong> el Responsable del tratamiento será responsable de asegurar que los principios anteriores se cumplen.</li>
                </ul>
                
                <h2>Categorías de datos personales</h2>
                <p>Las categorías de datos que se tratan en Instituto San Martín son únicamente datos identificativos. En ningún caso, se tratan categorías especiales de datos personales en el sentido del artículo 9 del RGPD.</p>
                
                <h2>Base legal para el tratamiento de los datos personales</h2>
                <p>La base legal para el tratamiento de los datos personales es el consentimiento. Instituto San Martín se compromete a recabar el consentimiento expreso y verificable del Usuario para el tratamiento de sus datos personales para uno o varios fines específicos.</p>
                <p>El Usuario tendrá derecho a retirar su consentimiento en cualquier momento. Será tan fácil retirar el consentimiento como darlo. Como regla general, la retirada del consentimiento no condicionará el uso del Sitio Web.</p>
                <p>En las ocasiones en las que el Usuario deba o pueda facilitar sus datos a través de formularios para realizar consultas, solicitar información o por motivos relacionados con el contenido del Sitio Web, se le informará en caso de que la cumplimentación de alguno de ellos sea obligatoria debido a que los mismos sean imprescindibles para el correcto desarrollo de la operación realizada.</p>
                
                <h2>Fines del tratamiento a que se destinan los datos personales</h2>
                <p>Los datos personales son recabados y gestionados por Instituto San Martín con la finalidad de poder facilitar, agilizar y cumplir los compromisos establecidos entre el Sitio Web y el Usuario o el mantenimiento de la relación que se establezca en los formularios que este último rellene o para atender una solicitud o consulta.</p>
                <p>Igualmente, los datos podrán ser utilizados con una finalidad comercial de personalización, operativa y estadística, y actividades propias del objeto social de Instituto San Martín, así como para la extracción, almacenamiento de datos y estudios de marketing para adecuar el Contenido ofertado al Usuario, así como mejorar la calidad, funcionamiento y navegación por el Sitio Web.</p>
                <p>En el momento en que se obtengan los datos personales, se informará al Usuario acerca del fin o fines específicos del tratamiento a que se destinarán los datos personales; es decir, del uso o usos que se dará a la información recopilada.</p>
                
                <h2>Períodos de retención de los datos personales</h2>
                <p>Los datos personales solo serán retenidos durante el tiempo mínimo necesario para los fines de su tratamiento y, en todo caso, únicamente durante el siguiente plazo: 1 año, o hasta que el Usuario solicite su supresión.</p>
                <p>En el momento en que se obtengan los datos personales, se informará al Usuario acerca del plazo durante el cual se conservarán los datos personales o, cuando eso no sea posible, los criterios utilizados para determinar este plazo.</p>
                
                <h2>Destinatarios de los datos personales</h2>
                <p>Los datos personales del Usuario serán compartidos con los siguientes destinatarios o categorías de destinatarios:</p>
                <ul>
                    <li>Gerard Durán López - Calle Andalucía Nº12</li>
                </ul>
                <p>En caso de que el Responsable del tratamiento tenga la intención de transferir datos personales a un tercer país u organización internacional, en el momento en que se obtengan los datos personales, se informará al Usuario acerca del tercer país u organización internacional al cual se tiene la intención de transferir los datos, así como de la existencia o ausencia de una decisión de adecuación de la Comisión.</p>
                
                <h2>Datos personales de menores de edad</h2>
                <p>Respetando lo establecido en los artículos 8 del RGPD y 7 de la Ley Orgánica 3/2018, de 5 de diciembre, de Protección de Datos Personales y garantía de los derechos digitales, solo los mayores de 14 años podrán otorgar su consentimiento para el tratamiento de sus datos personales de forma lícita por Instituto San Martín. Si se trata de un menor de 14 años, será necesario el consentimiento de los padres o tutores para el tratamiento, y este solo se considerará lícito en la medida en la que los mismos lo hayan autorizado.</p>
                
                <h2>Secreto y seguridad de los datos personales</h2>
                <p>Instituto San Martín se compromete a adoptar las medidas técnicas y organizativas necesarias, según el nivel de seguridad adecuado al riesgo de los datos recogidos, de forma que se garantice la seguridad de los datos de carácter personal y se evite la destrucción, pérdida o alteración accidental o ilícita de datos personales transmitidos, conservados o tratados de otra forma, o la comunicación o acceso no autorizados a dichos datos.</p>
                <p>El Sitio Web cuenta con un certificado SSL (Secure Socket Layer), que asegura que los datos personales se transmiten de forma segura y confidencial, al ser la transmisión de los datos entre el servidor y el Usuario, y en retroalimentación, totalmente cifrada o encriptada.</p>
                <p>Sin embargo, debido a que Instituto San Martín no puede garantizar la inexpugnabilidad de internet ni la ausencia total de hackers u otros que accedan de modo fraudulento a los datos personales, el Responsable del tratamiento se compromete a comunicar al Usuario sin dilación indebida cuando ocurra una violación de la seguridad de los datos personales que sea probable que entrañe un alto riesgo para los derechos y libertades de las personas físicas. Siguiendo lo establecido en el artículo 4 del RGPD, se entiende por violación de la seguridad de los datos personales toda violación de la seguridad que ocasione la destrucción, pérdida o alteración accidental o ilícita de datos personales transmitidos, conservados o tratados de otra forma, o la comunicación o acceso no autorizados a dichos datos.</p>
                <p>Los datos personales serán tratados como confidenciales por el Responsable del tratamiento, quien se compromete a informar de y a garantizar por medio de una obligación legal o contractual que dicha confidencialidad sea respetada por sus empleados, asociados, y toda persona a la cual le haga accesible la información.</p>
                
                <h2>Derechos derivados del tratamiento de los datos personales</h2>
                <p>El Usuario tiene sobre Instituto San Martín y podrá, por tanto, ejercer frente al Responsable del tratamiento los siguientes derechos reconocidos en el RGPD y la Ley Orgánica 3/2018, de 5 de diciembre, de Protección de Datos Personales y garantía de los derechos digitales:</p>
                <ul>
                    <li><strong>Derecho de acceso:</strong> Es el derecho del Usuario a obtener confirmación de si Instituto San Martín está tratando o no sus datos personales y, en caso afirmativo, obtener información sobre sus datos concretos de carácter personal y del tratamiento que Instituto San Martín haya realizado o realice, así como, entre otra, de la información disponible sobre el origen de dichos datos y los destinatarios de las comunicaciones realizadas o previstas de los mismos.</li>
                    <li><strong>Derecho de rectificación:</strong> Es el derecho del Usuario a que se modifiquen sus datos personales que resulten ser inexactos o, teniendo en cuenta los fines del tratamiento, incompletos.</li>
                    <li><strong>Derecho de supresión (el "derecho al olvido"):</strong> Es el derecho del Usuario, siempre que la legislación vigente no establezca lo contrario, a obtener la supresión de sus datos personales cuando estos ya no sean necesarios para los fines para los cuales fueron recogidos o tratados; el Usuario haya retirado su consentimiento al tratamiento y este no cuente con otra base legal; el Usuario se oponga al tratamiento y no exista otro motivo legítimo para continuar con el mismo; los datos personales hayan sido tratados ilícitamente; los datos personales deban suprimirse en cumplimiento de una obligación legal; o los datos personales hayan sido obtenidos producto de una oferta directa de servicios de la sociedad de la información a un menor de 14 años. Además de suprimir los datos, el Responsable del tratamiento, teniendo en cuenta la tecnología disponible y el coste de su aplicación, deberá adoptar medidas razonables para informar a los responsables que estén tratando los datos personales de la solicitud del interesado de supresión de cualquier enlace a esos datos personales.</li>
                    <li><strong>Derecho a la limitación del tratamiento:</strong> Es el derecho del Usuario a limitar el tratamiento de sus datos personales. El Usuario tiene derecho a obtener la limitación del tratamiento cuando impugne la exactitud de sus datos personales; el tratamiento sea ilícito; el Responsable del tratamiento ya no necesite los datos personales, pero el Usuario lo necesite para hacer reclamaciones; y cuando el Usuario se haya opuesto al tratamiento.</li>
                    <li><strong>Derecho a la portabilidad de los datos:</strong> En caso de que el tratamiento se efectúe por medios automatizados, el Usuario tendrá derecho a recibir del Responsable del tratamiento sus datos personales en un formato estructurado, de uso común y lectura mecánica, y a transmitirlos a otro responsable del tratamiento. Siempre que sea técnicamente posible, el Responsable del tratamiento transmitirá directamente los datos a ese otro responsable.</li>
                    <li><strong>Derecho de oposición:</strong> Es el derecho del Usuario a que no se lleve a cabo el tratamiento de sus datos de carácter personal o se cese el tratamiento de los mismos por parte de Instituto San Martín.</li>
                    <li><strong>Derecho a no ser objeto de una decisión basada únicamente en el tratamiento automatizado, incluida la elaboración de perfiles:</strong> Es el derecho del Usuario a no ser objeto de una decisión individualizada basada únicamente en el tratamiento automatizado de sus datos personales, incluida la elaboración de perfiles, existente salvo que la legislación vigente establezca lo contrario.</li>
                </ul>
                <p>Así pues, el Usuario podrá ejercitar sus derechos mediante comunicación escrita dirigida al Responsable del tratamiento con la referencia "RGPD-V", especificando:</p>
                <ul>
                    <li>Nombre, apellidos del Usuario y copia del DNI. En los casos en que se admita la representación, será también necesaria la identificación por el mismo medio de la persona que representa al Usuario, así como el documento acreditativo de la representación. La fotocopia del DNI podrá ser sustituida, por cualquier otro medio válido en derecho que acredite la identidad.</li>
                    <li>Petición con los motivos específicos de la solicitud o información a la que se quiere acceder.</li>
                    <li>Domicilio a efecto de notificaciones.</li>
                    <li>Fecha y firma del solicitante.</li>
                    <li>Todo documento que acredite la petición que formula.</li>
                </ul>
                <p>Esta solicitud y todo otro documento adjunto podrá enviarse a la siguiente dirección y/o correo electrónico:</p>
                <ul>
                    <li><strong>Dirección postal:</strong> Calle Andalusia Nº12</li>
                    <li><strong>Correo electrónico:</strong> milaloab240681@gmail.com</li>
                </ul>
                
                <h2>Enlaces a sitios web de terceros</h2>
                <p>El Sitio Web puede incluir hipervínculos o enlaces que permiten acceder a páginas web de terceros distintos de Instituto San Martín, y que por tanto no son operados por Instituto San Martín. Los titulares de dichos sitios web dispondrán de sus propias políticas de protección de datos, siendo ellos mismos, en cada caso, responsables de sus propios ficheros y de sus propias prácticas de privacidad.</p>
                
                <h2>Reclamaciones ante la autoridad de control</h2>
                <p>En caso de que el Usuario considere que existe un problema o infracción de la normativa vigente en la forma en la que se están tratando sus datos personales, tendrá derecho a la tutela judicial efectiva y a presentar una reclamación ante una autoridad de control, en particular, en el Estado en el que tenga su residencia habitual, lugar de trabajo o lugar de la supuesta infracción. En el caso de España, la autoridad de control es la Agencia Española de Protección de Datos (https://www.aepd.es).</p>
                
                <h2>II. ACEPTACIÓN Y CAMBIOS EN ESTA POLÍTICA DE PRIVACIDAD</h2>
                <p>Es necesario que el Usuario haya leído y esté conforme con las condiciones sobre la protección de datos de carácter personal contenidas en esta Política de Privacidad, así como que acepte el tratamiento de sus datos personales para que el Responsable del tratamiento pueda proceder al mismo en la forma, durante los plazos y para las finalidades indicadas. El uso del Sitio Web implicará la aceptación de la Política de Privacidad del mismo.</p>
                <p>Instituto San Martín se reserva el derecho a modificar su Política de Privacidad, de acuerdo a su propio criterio, o motivado por un cambio legislativo, jurisprudencial o doctrinal de la Agencia Española de Protección de Datos. Los cambios o actualizaciones de esta Política de Privacidad no serán notificados de forma explícita al Usuario. Se recomienda al Usuario consultar esta página de forma periódica para estar al tanto de los últimos cambios o actualizaciones.</p>
                <p>Esta Política de Privacidad fue actualizada para adaptarse al Reglamento (UE) 2016/679 del Parlamento Europeo y del Consejo, de 27 de abril de 2016, relativo a la protección de las personas físicas en lo que respecta al tratamiento de datos personales y a la libre circulación de estos datos (RGPD) y a la Ley Orgánica 3/2018, de 5 de diciembre, de Protección de Datos Personales y garantía de los derechos digitales.</p>
                <p class="text-muted small mt-4">Este documento de Política de Privacidad de un sitio web ha sido creado mediante el generador de plantilla de política de privacidad web gratis online el día 09/12/2025.</p>
                
                <div class="d-flex justify-content-center gap-3 mt-5">
                    <button id="acceptPrivacyBtn" class="btn btn-custom-primary">Aceptar</button>
                    <button class="btn btn-outline-secondary" onclick="closeModal('privacyPolicyModal')">Cerrar</button>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal de Excelencia Académica -->
    <div id="modal-excelencia" class="custom-modal">
        <div class="custom-modal-content">
            <button class="btn-close position-absolute top-0 end-0 m-3" onclick="closeModal('modal-excelencia')"></button>
            <div class="p-4">
                <div class="card-icon mx-auto mb-4">
                    <svg xmlns="http://www.w3.org/2000/svg" width="40" height="40" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                        <circle cx="12" cy="8" r="7"/>
                        <polyline points="8.21 13.89 7 23 12 20 17 23 15.79 13.88"/>
                    </svg>
                </div>
                <h2 class="text-primary text-center">Excelencia Académica</h2>
                
                <h3>Nuestro Compromiso</h3>
                <p>En el Instituto San Martín, la excelencia académica es nuestro principal compromiso. Contamos con:</p>
                
                <ul>
                    <li><strong>Plan de estudios actualizado:</strong> Basado en las últimas investigaciones educativas y necesidades del mercado laboral.</li>
                    <li><strong>Razón alumno-profesor:</strong> 15:1 para garantizar atención personalizada.</li>
                    <li><strong>Tutorías individualizadas:</strong> Cada estudiante tiene asignado un tutor que sigue su progreso.</li>
                    <li><strong>Evaluación continua:</strong> Sistema de evaluación formativa que valora el proceso de aprendizaje.</li>
                    <li><strong>Preparación integral:</strong> Para pruebas nacionales e internacionales.</li>
                </ul>
                
                <h3>Resultados</h3>
                <p>Nuestros resultados hablan por sí solos:</p>
                <ul>
                    <li>95% de nuestros estudiantes ingresan a la universidad de su primera opción.</li>
                    <li>Premio a la Excelencia Educativa 2022 y 2023.</li>
                    <li>Reconocimiento como "Institución de Referencia" por el Ministerio de Educación.</li>
                </ul>
                
                <div class="text-center mt-4">
                    <button class="btn btn-custom-primary" onclick="closeModal('modal-excelencia')">Entendido</button>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal de Educación Primaria -->
    <div id="modal-primaria" class="custom-modal">
        <div class="custom-modal-content">
            <button class="btn-close position-absolute top-0 end-0 m-3" onclick="closeModal('modal-primaria')"></button>
            <div class="p-4">
                <h2 class="text-primary">Educación Primaria</h2>
                
                <h3>Programa Integral (6-12 años)</h3>
                <p>Nuestro programa de Educación Primaria está diseñado para desarrollar las habilidades fundamentales en un ambiente seguro y estimulante.</p>
                
                <h3>Características Principales</h3>
                <ul>
                    <li><strong>Horario:</strong> 8:00 - 14:00 (con opción de horario extendido hasta 17:00)</li>
                    <li><strong>Inglés intensivo:</strong> 10 horas semanales con profesores nativos</li>
                    <li><strong>Tecnología educativa:</strong> Tablets y pizarras digitales en todas las aulas</li>
                    <li><strong>Educación emocional:</strong> Programa de inteligencia emocional integrado</li>
                    <li><strong>Deportes y arte:</strong> 4 horas semanales de educación física y 3 de artes</li>
                </ul>
                
                <h3>Metodología</h3>
                <p>Utilizamos metodologías activas como:</p>
                <ul>
                    <li>Aprendizaje basado en proyectos</li>
                    <li>Trabajo cooperativo</li>
                    <li>Gamificación educativa</li>
                    <li>Rincones de aprendizaje</li>
                </ul>
                
                <h3>Actividades Complementarias</h3>
                <ul>
                    <li>Talleres de robótica y programación</li>
                    <li>Clubes de lectura y escritura creativa</li>
                    <li>Excursiones educativas mensuales</li>
                    <li>Olimpiadas matemáticas y científicas</li>
                </ul>
                
                <div class="text-center mt-4">
                    <button class="btn btn-custom-primary" onclick="closeModal('modal-primaria'); scrollToSection('contacto')">Solicitar Información</button>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal de Instalaciones -->
    <div id="modal-instalaciones" class="custom-modal">
        <div class="custom-modal-content">
            <button class="btn-close position-absolute top-0 end-0 m-3" onclick="closeModal('modal-instalaciones')"></button>
            <div class="p-4">
                <h2 class="text-primary">Nuestras Instalaciones</h2>
                
                <h3>Campus Principal</h3>
                <p>Nuestro campus de 25,000 m² está diseñado para optimizar el aprendizaje y desarrollo integral.</p>
                
                <h3>Infraestructura Académica</h3>
                <ul>
                    <li><strong>32 aulas inteligentes:</strong> Equipadas con tecnología de punta</li>
                    <li><strong>8 laboratorios:</strong> Ciencias, física, química, biología y tecnología</li>
                    <li><strong>Biblioteca:</strong> 15,000 volúmenes + plataforma digital con 50,000 recursos</li>
                    <li><strong>Aulas especializadas:</strong> Música, arte, tecnología y robótica</li>
                    <li><strong>Salón de usos múltiples:</strong> Capacidad para 500 personas</li>
                </ul>
                
                <h3>Instalaciones Deportivas</h3>
                <ul>
                    <li>Cancha de fútbol profesional</li>
                    <li>Piscina semiolímpica climatizada</li>
                    <li>Gimnasio multiusos</li>
                    <li>Canchas de baloncesto y voleibol</li>
                    <li>Pista de atletismo</li>
                </ul>
                
                <h3>Áreas Recreativas</h3>
                <ul>
                    <li>Patios diferenciados por edades</li>
                    <li>Áreas verdes y jardín botánico</li>
                    <li>Comedor con capacidad para 800 estudiantes</li>
                    <li>Enfermería con atención permanente</li>
                    <li>Auditorio para 300 personas</li>
                </ul>
                
                <div class="text-center mt-4">
                    <button class="btn btn-custom-primary" onclick="closeModal('modal-instalaciones')">Entendido</button>
                </div>
            </div>
        </div>
    </div>

    <!-- Navegación -->
    <nav class="navbar navbar-expand-lg navbar-light bg-white fixed-top shadow-sm py-3" id="navbar">
        <div class="container">
            <a href="#inicio" class="navbar-brand d-flex align-items-center">
                <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="me-2">
                    <path d="M22 10v6M2 10l10-5 10 5-10 5z"/>
                    <path d="M6 12v5c3 3 9 3 12 0v-5"/>
                </svg>
                Instituto San Martín
            </a>

            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>

            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto align-items-center">
                    <li class="nav-item"><button class="nav-link btn btn-link" onclick="scrollToSection('inicio')">Inicio</button></li>
                    <li class="nav-item"><button class="nav-link btn btn-link" onclick="scrollToSection('nosotros')">Nosotros</button></li>
                    <li class="nav-item"><button class="nav-link btn btn-link" onclick="scrollToSection('programas')">Programas</button></li>
                    <li class="nav-item"><button class="nav-link btn btn-link" onclick="scrollToSection('instalaciones')">Instalaciones</button></li>
                    <li class="nav-item"><button class="nav-link btn btn-link" onclick="scrollToSection('contacto')">Contacto</button></li>
                    <li class="nav-item ms-2"><button class="btn btn-custom-primary" onclick="scrollToSection('contacto')">Inscríbete</button></li>
                </ul>
            </div>
        </div>
    </nav>

    <!-- Sección Hero -->
    <section id="inicio" class="hero d-flex align-items-center justify-content-center">
        <div class="hero-content text-center">
            <h1>Formando Líderes del Mañana</h1>
            <p class="hero-subtitle">Excelencia académica, valores sólidos y formación integral desde 1985</p>
            <div class="d-flex gap-3 justify-content-center flex-wrap">
                <button class="btn btn-custom-primary btn-lg d-flex align-items-center gap-2" onclick="scrollToSection('programas')">
                    Ver Programas
                    <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                        <path d="M5 12h14"/>
                        <path d="m12 5 7 7-7 7"/>
                    </svg>
                </button>
                <button class="btn btn-custom-outline btn-lg" onclick="scrollToSection('contacto')">Contáctanos</button>
            </div>
        </div>
        
        <!-- Scroll indicator -->
        <div class="position-absolute bottom-0 start-50 translate-middle-x mb-4">
            <button onclick="scrollToSection('nosotros')" class="btn btn-link text-white">
                <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                    <path d="M12 5v14"/>
                    <path d="m19 12-7 7-7-7"/>
                </svg>
            </button>
        </div>
    </section>

    <!-- Sección Nosotros -->
    <section id="nosotros" class="section section-bg">
        <div class="container">
            <div class="text-center mb-5">
                <h2 class="text-center">Sobre Nosotros</h2>
                <p class="lead">Más de 35 años formando líderes con valores y excelencia académica</p>
            </div>

            <div class="row g-4">
                <div class="col-md-6 col-lg-3">
                    <div class="custom-card" onclick="openModal('modal-excelencia')">
                        <div class="card-icon mx-auto mt-4">
                            <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                <circle cx="12" cy="8" r="7"/>
                                <polyline points="8.21 13.89 7 23 12 20 17 23 15.79 13.88"/>
                            </svg>
                        </div>
                        <div class="custom-card-content">
                            <h3 class="text-center">Excelencia Académica</h3>
                            <p class="text-center">Programas educativos de alta calidad con enfoque en el desarrollo integral del estudiante.</p>
                            <p class="text-center text-primary mt-auto mb-0 small">Click para más información</p>
                        </div>
                    </div>
                </div>
                
                <div class="col-md-6 col-lg-3">
                    <div class="custom-card">
                        <div class="card-icon mx-auto mt-4">
                            <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                <path d="M16 21v-2a4 4 0 0 0-4-4H6a4 4 0 0 0-4 4v2"/>
                                <circle cx="9" cy="7" r="4"/>
                                <path d="M22 21v-2a4 4 0 0 0-3-3.87"/>
                                <path d="M16 3.13a4 4 0 0 1 0 7.75"/>
                            </svg>
                        </div>
                        <div class="custom-card-content">
                            <h3 class="text-center">Comunidad Inclusiva</h3>
                            <p class="text-center">Ambiente de respeto mutuo, trabajo en equipo y colaboración entre estudiantes, profesores y familias.</p>
                            <p class="text-center"><strong>50+ clubes estudiantiles</strong> y programas de voluntariado activos.</p>
                        </div>
                    </div>
                </div>
                
                <div class="col-md-6 col-lg-3">
                    <div class="custom-card">
                        <div class="card-icon mx-auto mt-4">
                            <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                <path d="M4 19.5A2.5 2.5 0 0 1 6.5 17H20"/>
                                <path d="M6.5 2H20v20H6.5A2.5 2.5 0 0 1 4 19.5v-15A2.5 2.5 0 0 1 6.5 2z"/>
                            </svg>
                        </div>
                        <div class="custom-card-content">
                            <h3 class="text-center">Innovación Educativa</h3>
                            <p class="text-center">Métodos de enseñanza modernos adaptados al siglo XXI y tecnología de vanguardia en todas las aulas.</p>
                            <p class="text-center"><strong>Certificación Google Reference School</strong> desde 2020.</p>
                        </div>
                    </div>
                </div>
                
                <div class="col-md-6 col-lg-3">
                    <div class="custom-card">
                        <div class="card-icon mx-auto mt-4">
                            <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                <path d="M20.42 4.58a5.4 5.4 0 0 0-7.65 0l-.77.78-.77-.78a5.4 5.4 0 0 0-7.65 0C1.46 6.7 1.33 10.28 4 13l8 8 8-8c2.67-2.72 2.54-6.3.42-8.42z"/>
                            </svg>
                        </div>
                        <div class="custom-card-content">
                            <h3 class="text-center">Valores y Ética</h3>
                            <p class="text-center">Formación en principios éticos, responsabilidad social y compromiso con la comunidad.</p>
                            <p class="text-center"><strong>10,000+ horas anuales</strong> de voluntariado estudiantil.</p>
                        </div>
                    </div>
                </div>
            </div>

            <div class="row g-4 mt-5">
                <div class="col-md-4">
                    <div class="stat-item">
                        <div class="stat-number" data-count="1500">0</div>
                        <p>Estudiantes Activos</p>
                        <p class="small text-muted">Distribuidos en todos los niveles educativos</p>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="stat-item">
                        <div class="stat-number" data-count="150">0</div>
                        <p>Docentes Calificados</p>
                        <p class="small text-muted">80% con maestría o doctorado</p>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="stat-item">
                        <div class="stat-number" data-count="98">0</div>
                        <p>% Tasa de Graduación</p>
                        <p class="small text-muted">Promedio últimos 5 años</p>
                    </div>
                </div>
            </div>

            <div class="mt-5 p-4 bg-white rounded-3 shadow-sm">
                <h3 class="text-center mb-4">Nuestra Historia</h3>
                <p>Fundado en 1985 por un grupo de educadores visionarios, el Instituto San Martín nació con la misión de transformar la educación en nuestra comunidad. Lo que comenzó como una pequeña escuela con 50 estudiantes, hoy es una institución de referencia con más de 1,500 alumnos.</p>
                <p>A lo largo de 35 años, hemos mantenido nuestro compromiso con la excelencia académica mientras nos adaptamos a los cambios tecnológicos y sociales. Hemos sido pioneros en la implementación de tecnología educativa, programas bilingües y educación emocional.</p>
                <p>Nuestros egresados han destacado en diversas áreas: científicos premiados, empresarios exitosos, artistas reconocidos y líderes comunitarios. Este legado nos motiva a seguir innovando y mejorando cada día.</p>
            </div>
        </div>
    </section>

    <!-- Sección Programas -->
    <section id="programas" class="section">
        <div class="container">
            <div class="text-center mb-5">
                <h2 class="text-center">Nuestros Programas</h2>
                <p class="lead">Programas educativos innovadores adaptados a las necesidades del siglo XXI</p>
            </div>

            <div class="row g-4">
                <div class="col-md-6 col-lg-4">
                    <div class="custom-card" onclick="openModal('modal-primaria')">
                        <div class="custom-card-content">
                            <div class="d-flex justify-content-center mb-3">
                                <div class="card-icon-sm">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                        <path d="M22 10v6M2 10l10-5 10 5-10 5z"/>
                                        <path d="M6 12v5c3 3 9 3 12 0v-5"/>
                                    </svg>
                                </div>
                            </div>
                            <h3 class="text-center">Educación Primaria</h3>
                            <p class="text-center"><strong>Edades:</strong> 6 a 12 años</p>
                            <p class="text-center">Programa integral con enfoque en habilidades fundamentales, inglés intensivo y desarrollo emocional.</p>
                            <ul class="mt-2">
                                <li>Inglés: 10 horas semanales</li>
                                <li>Tecnología educativa integrada</li>
                                <li>Programa de inteligencia emocional</li>
                            </ul>
                            <p class="text-center text-primary mt-auto mb-0 small">Click para detalles completos</p>
                        </div>
                    </div>
                </div>
                
                <div class="col-md-6 col-lg-4">
                    <div class="custom-card">
                        <div class="custom-card-content">
                            <div class="d-flex justify-content-center mb-3">
                                <div class="card-icon-sm">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                        <rect x="3" y="3" width="18" height="18" rx="2" ry="2"/>
                                        <line x1="3" y1="9" x2="21" y2="9"/>
                                        <line x1="9" y1="21" x2="9" y2="9"/>
                                    </svg>
                                </div>
                            </div>
                            <h3 class="text-center">Educación Secundaria</h3>
                            <p class="text-center"><strong>Edades:</strong> 12 a 18 años</p>
                            <p class="text-center">Preparación académica sólida con orientación vocacional y preparación universitaria.</p>
                            <ul class="mt-2">
                                <li>Programa de orientación vocacional</li>
                                <li>Certificaciones internacionales</li>
                                <li>Proyectos de investigación</li>
                            </ul>
                            <p class="text-center"><strong>Horario:</strong> 7:30 - 15:30</p>
                        </div>
                    </div>
                </div>
                
                <div class="col-md-6 col-lg-4">
                    <div class="custom-card">
                        <div class="custom-card-content">
                            <div class="d-flex justify-content-center mb-3">
                                <div class="card-icon-sm">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                        <path d="M6 2 3 6v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2V6l-3-4z"/>
                                        <line x1="3" y1="6" x2="21" y2="6"/>
                                        <path d="M16 10a4 4 0 0 1-8 0"/>
                                    </svg>
                                </div>
                            </div>
                            <h3 class="text-center">Bachillerato en Ciencias</h3>
                            <p class="text-center"><strong>Duración:</strong> 2 años</p>
                            <p class="text-center">Especialización en ciencias naturales, matemáticas y tecnología con laboratorios equipados.</p>
                            <ul class="mt-2">
                                <li>Laboratorios de última generación</li>
                                <li>Proyectos STEM avanzados</li>
                                <li>Preparación para carreras científicas</li>
                            </ul>
                            <p class="text-center"><strong>Titulación:</strong> Bachiller en Ciencias</p>
                        </div>
                    </div>
                </div>
                
                <div class="col-md-6 col-lg-4">
                    <div class="custom-card">
                        <div class="custom-card-content">
                            <div class="d-flex justify-content-center mb-3">
                                <div class="card-icon-sm">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                        <circle cx="12" cy="12" r="10"/>
                                        <line x1="2" y1="12" x2="22" y2="12"/>
                                        <path d="M12 2a15.3 15.3 0 0 1 4 10 15.3 15.3 0 0 1-4 10 15.3 15.3 0 0 1-4-10 15.3 15.3 0 0 1 4-10z"/>
                                    </svg>
                                </div>
                            </div>
                            <h3 class="text-center">Bachillerato en Humanidades</h3>
                            <p class="text-center"><strong>Duración:</strong> 2 años</p>
                            <p class="text-center">Enfoque en ciencias sociales, lenguas y comunicación con perspectiva global.</p>
                            <ul class="mt-2">
                                <li>Tres idiomas extranjeros</li>
                                <li>Debates y oratoria</li>
                                <li>Estudios culturales internacionales</li>
                            </ul>
                            <p class="text-center"><strong>Titulación:</strong> Bachiller en Humanidades</p>
                        </div>
                    </div>
                </div>
                
                <div class="col-md-6 col-lg-4">
                    <div class="custom-card">
                        <div class="custom-card-content">
                            <div class="d-flex justify-content-center mb-3">
                                <div class="card-icon-sm">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                        <rect x="3" y="3" width="18" height="18" rx="2" ry="2"/>
                                        <circle cx="9" cy="9" r="2"/>
                                        <path d="m21 15-3.086-3.086a2 2 0 0 0-2.828 0L6 21"/>
                                    </svg>
                                </div>
                            </div>
                            <h3 class="text-center">Programa de Artes</h3>
                            <p class="text-center">Desarrollo de habilidades artísticas y creatividad para todos los niveles.</p>
                            <ul class="mt-2">
                                <li>Artes plásticas y visuales</li>
                                <li>Teatro y expresión corporal</li>
                                <li>Música y danza</li>
                                <li>Exposiciones anuales</li>
                            </ul>
                            <p class="text-center"><strong>Instalaciones:</strong> Talleres de arte completamente equipados</p>
                        </div>
                    </div>
                </div>
                
                <div class="col-md-6 col-lg-4">
                    <div class="custom-card">
                        <div class="custom-card-content">
                            <div class="d-flex justify-content-center mb-3">
                                <div class="card-icon-sm">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                        <path d="M9 18V5l12-2v13"/>
                                        <circle cx="6" cy="18" r="3"/>
                                        <circle cx="18" cy="16" r="3"/>
                                    </svg>
                                </div>
                            </div>
                            <h3 class="text-center">Programa Musical</h3>
                            <p class="text-center">Formación en teoría musical e interpretación instrumental desde nivel básico a avanzado.</p>
                            <ul class="mt-2">
                                <li>Clases individuales y grupales</li>
                                <li>Orquesta y coro estudiantil</li>
                                <li>Conciertos públicos trimestrales</li>
                                <li>Grabación en estudio profesional</li>
                            </ul>
                            <p class="text-center"><strong>Instrumentos:</strong> 15+ instrumentos disponibles</p>
                        </div>
                    </div>
                </div>
            </div>

            <div class="mt-4 p-4 bg-light rounded-3">
                <h3 class="text-center">Programas Especiales</h3>
                <div class="row g-4 mt-3">
                    <div class="col-md-4">
                        <h4>Programa Deportivo</h4>
                        <p>Entrenamiento en fútbol, baloncesto, natación y atletismo con coaches profesionales.</p>
                    </div>
                    <div class="col-md-4">
                        <h4>Robótica y Programación</h4>
                        <p>Desde robótica básica hasta programación avanzada y desarrollo de apps.</p>
                    </div>
                    <div class="col-md-4">
                        <h4>Intercambios Internacionales</h4>
                        <p>Programas de intercambio con escuelas en EE.UU., Canadá, España y Australia.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Sección Instalaciones -->
    <section id="instalaciones" class="section section-bg">
        <div class="container">
            <div class="text-center mb-5">
                <h2 class="text-center">Nuestras Instalaciones</h2>
                <p class="lead">Infraestructura de primer nivel para un aprendizaje óptimo y desarrollo integral</p>
            </div>

            <div class="row g-4">
                <div class="col-lg-6">
                    <div class="custom-card" onclick="openModal('modal-instalaciones')">
                        <img src="https://images.unsplash.com/photo-1654366698665-e6d611a9aaa9?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&q=80&w=1080" alt="Aulas Modernas" class="custom-card-img">
                        <div class="custom-card-content">
                            <h3>Aulas Inteligentes</h3>
                            <p>32 aulas equipadas con tecnología de punta: pizarras digitales interactivas, sistemas de sonido, proyectores 4K y conexión WiFi de alta velocidad.</p>
                            <p><strong>Capacidad:</strong> 25 estudiantes por aula</p>
                            <p><strong>Características:</strong> Iluminación LED regulable, climatización individual, mobiliario ergonómico</p>
                            <p class="text-primary small">Click para ver todas las instalaciones</p>
                        </div>
                    </div>
                </div>
                
                <div class="col-lg-6">
                    <div class="custom-card">
                        <img src="https://images.unsplash.com/photo-1706528010331-0f12582db334?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&q=80&w=1080" alt="Biblioteca" class="custom-card-img">
                        <div class="custom-card-content">
                            <h3>Biblioteca y Centro de Recursos</h3>
                            <p>Más de 15,000 volúmenes físicos + acceso a plataforma digital con 50,000 recursos académicos.</p>
                            <p><strong>Áreas:</strong> Sala de lectura silenciosa, área de estudio grupal, zona multimedia, hemeroteca</p>
                            <p><strong>Horario:</strong> 7:30 - 19:00 de lunes a viernes</p>
                            <p><strong>Servicios:</strong> Préstamo de libros, acceso a bases de datos, talleres de investigación</p>
                        </div>
                    </div>
                </div>
                
                <div class="col-lg-6">
                    <div class="custom-card">
                        <img src="https://images.unsplash.com/photo-1602052577122-f73b9710adba?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&q=80&w=1080" alt="Laboratorios" class="custom-card-img">
                        <div class="custom-card-content">
                            <h3>Laboratorios Científicos</h3>
                            <p>8 laboratorios completamente equipados para experimentación práctica en todas las áreas científicas.</p>
                            <p><strong>Laboratorios:</strong> Biología, Química, Física, Tecnología, Robótica, Ciencias de la Computación</p>
                            <p><strong>Equipamiento:</strong> Microscopios electrónicos, espectrómetros, kits de robótica, impresoras 3D</p>
                            <p><strong>Seguridad:</strong> Cumplimiento de normas internacionales de seguridad</p>
                        </div>
                    </div>
                </div>
                
                <div class="col-lg-6">
                    <div class="custom-card">
                        <img src="https://images.unsplash.com/photo-1565673686362-85864074640a?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&q=80&w=1080" alt="Instalaciones Deportivas" class="custom-card-img">
                        <div class="custom-card-content">
                            <h3>Instalaciones Deportivas</h3>
                            <p>Complejo deportivo de 8,000 m² para el desarrollo físico y competencias deportivas.</p>
                            <p><strong>Cancha principal:</strong> Fútbol 11 con césped artificial</p>
                            <p><strong>Piscina:</strong> Semiolímpica climatizada (25m x 6 carriles)</p>
                            <p><strong>Gimnasio:</strong> Multiusos para baloncesto, voleibol y badminton</p>
                            <p><strong>Otros:</strong> Pista de atletismo, canchas de tenis, sala de fitness</p>
                        </div>
                    </div>
                </div>
            </div>

            <div class="mt-4 p-4 bg-white rounded-3 shadow-sm">
                <h3 class="text-center">Servicios Adicionales</h3>
                <div class="row g-4 mt-3">
                    <div class="col-md-4">
                        <h4>Comedor Escolar</h4>
                        <p>Servicio de comedor con capacidad para 800 estudiantes. Menús supervisados por nutricionistas.</p>
                    </div>
                    <div class="col-md-4">
                        <h4>Transporte Escolar</h4>
                        <p>Rutas cubriendo toda el área metropolitana. Flota de 15 buses con todas las medidas de seguridad.</p>
                    </div>
                    <div class="col-md-4">
                        <h4>Enfermería</h4>
                        <p>Atención médica permanente con enfermera titulada. Convenio con hospital local para emergencias.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Sección Testimonios -->
    <section class="section section-accent">
        <div class="container">
            <div class="text-center mb-5">
                <h2 class="text-white text-center">Lo Que Dicen de Nosotros</h2>
                <p class="text-white">Testimonios de nuestra comunidad educativa</p>
            </div>

            <div class="row g-4">
                <div class="col-md-4">
                    <div class="testimonial-card">
                        <div class="quote-icon">
                            <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                <path d="M3 21c3 0 7-1 7-8V5c0-1.25-.756-2.017-2-2H4c-1.25 0-2 .75-2 1.972V11c0 1.25.75 2 2 2 1 0 1 0 1 1v1c0 1-1 2-2 2s-1 .008-1 1.031V20c0 1 0 1 1 1z"/>
                                <path d="M15 21c3 0 7-1 7-8V5c0-1.25-.757-2.017-2-2h-4c-1.25 0-2 .75-2 1.972V11c0 1.25.75 2 2 2h.75c0 2.25.25 4-2.75 4v3c0 1 0 1 1 1z"/>
                            </svg>
                        </div>
                        <p class="testimonial-text">"El Instituto San Martín ha sido fundamental en el desarrollo de mi hija. Los profesores son dedicados y el ambiente es excepcional. La atención personalizada que recibe ha hecho una gran diferencia en su aprendizaje."</p>
                        <div>
                            <p class="author-name">María González</p>
                            <p class="author-role">Madre de estudiante de Primaria</p>
                        </div>
                    </div>
                </div>
                
                <div class="col-md-4">
                    <div class="testimonial-card">
                        <div class="quote-icon">
                            <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                <path d="M3 21c3 0 7-1 7-8V5c0-1.25-.756-2.017-2-2H4c-1.25 0-2 .75-2 1.972V11c0 1.25.75 2 2 2 1 0 1 0 1 1v1c0 1-1 2-2 2s-1 .008-1 1.031V20c0 1 0 1 1 1z"/>
                                <path d="M15 21c3 0 7-1 7-8V5c0-1.25-.757-2.017-2-2h-4c-1.25 0-2 .75-2 1.972V11c0 1.25.75 2 2 2h.75c0 2.25.25 4-2.75 4v3c0 1 0 1 1 1z"/>
                            </svg>
                        </div>
                        <p class="testimonial-text">"Gracias a la preparación que recibí, pude ingresar a la universidad de mis sueños. El instituto me dio todas las herramientas necesarias no solo académicas, sino también de liderazgo y trabajo en equipo."</p>
                        <div>
                            <p class="author-name">Carlos Ramírez</p>
                            <p class="author-role">Egresado 2023 - Actualmente en Medicina</p>
                        </div>
                    </div>
                </div>
                
                <div class="col-md-4">
                    <div class="testimonial-card">
                        <div class="quote-icon">
                            <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                <path d="M3 21c3 0 7-1 7-8V5c0-1.25-.756-2.017-2-2H4c-1.25 0-2 .75-2 1.972V11c0 1.25.75 2 2 2 1 0 1 0 1 1v1c0 1-1 2-2 2s-1 .008-1 1.031V20c0 1 0 1 1 1z"/>
                                <path d="M15 21c3 0 7-1 7-8V5c0-1.25-.757-2.017-2-2h-4c-1.25 0-2 .75-2 1.972V11c0 1.25.75 2 2 2h.75c0 2.25.25 4-2.75 4v3c0 1 0 1 1 1z"/>
                            </svg>
                        </div>
                        <p class="testimonial-text">"Trabajar aquí es un privilegio. La institución apoya la innovación educativa y el desarrollo profesional constante. Los recursos disponibles y el ambiente colaborativo hacen que cada día sea una oportunidad de crecimiento."</p>
                        <div>
                            <p class="author-name">Ana Martínez</p>
                            <p class="author-role">Docente de Ciencias - 8 años en la institución</p>
                        </div>
                    </div>
                </div>
            </div>

            <div class="mt-5 text-center">
                <h3 class="text-white mb-4">Reconocimientos y Certificaciones</h3>
                <div class="d-flex flex-wrap justify-content-center gap-3">
                    <div class="bg-white-10 p-3 rounded-3" style="min-width: 200px; background: rgba(255,255,255,0.1);">
                        <p class="text-white fw-bold mb-1">Excelencia Educativa 2022</p>
                        <p class="text-primary-light small mb-0">Ministerio de Educación</p>
                    </div>
                    <div class="bg-white-10 p-3 rounded-3" style="min-width: 200px; background: rgba(255,255,255,0.1);">
                        <p class="text-white fw-bold mb-1">Google Reference School</p>
                        <p class="text-primary-light small mb-0">Certificación desde 2020</p>
                    </div>
                    <div class="bg-white-10 p-3 rounded-3" style="min-width: 200px; background: rgba(255,255,255,0.1);">
                        <p class="text-white fw-bold mb-1">Institución de Referencia</p>
                        <p class="text-primary-light small mb-0">Calificación 2021-2023</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Sección Contacto -->
    <section id="contacto" class="section">
        <div class="container">
            <div class="text-center mb-5">
                <h2 class="text-center">Contáctanos</h2>
                <p class="lead">¿Tienes preguntas? Estamos aquí para ayudarte. Completa el formulario o visítanos en nuestras instalaciones.</p>
            </div>

            <div class="row g-4">
                <div class="col-lg-6">
                    <div class="card border-0 shadow-sm">
                        <div class="card-body p-4">
                            <h3 class="mb-4">Envía un Mensaje</h3>
                            <form id="contactForm" class="custom-form">
                                <div class="mb-3">
                                    <label for="name" class="form-label">Nombre Completo *</label>
                                    <input type="text" class="form-control" id="name" name="name" placeholder="Tu nombre" required>
                                </div>
                                <div class="mb-3">
                                    <label for="email" class="form-label">Correo Electrónico *</label>
                                    <input type="email" class="form-control" id="email" name="email" placeholder="tu@email.com" required>
                                </div>
                                <div class="mb-3">
                                    <label for="phone" class="form-label">Teléfono</label>
                                    <input type="tel" class="form-control" id="phone" name="phone" placeholder="+54 11 1234-5678">
                                </div>
                                <div class="mb-3">
                                    <label for="program" class="form-label">Programa de Interés *</label>
                                    <select class="form-select" id="program" name="program" required>
                                        <option value="">Selecciona un programa</option>
                                        <option value="primaria">Educación Primaria</option>
                                        <option value="secundaria">Educación Secundaria</option>
                                        <option value="ciencias">Bachillerato en Ciencias</option>
                                        <option value="humanidades">Bachillerato en Humanidades</option>
                                        <option value="artes">Programa de Artes</option>
                                        <option value="musica">Programa Musical</option>
                                        <option value="otros">Otros programas</option>
                                    </select>
                                </div>
                                <div class="mb-4">
                                    <label for="message" class="form-label">Mensaje *</label>
                                    <textarea class="form-control" id="message" name="message" rows="4" placeholder="Escribe tu mensaje aquí..." required></textarea>
                                </div>
                                <button type="submit" class="btn btn-custom-primary w-100">Enviar Mensaje</button>
                            </form>
                        </div>
                    </div>
                </div>

                <div class="col-lg-6">
                    <div class="card border-0 shadow-sm mb-4">
                        <div class="card-body p-4">
                            <h3 class="mb-4">Información de Contacto</h3>
                            <div class="d-flex flex-column gap-4">
                                <div class="d-flex align-items-start gap-3">
                                    <div class="icon-container">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                            <path d="M20 10c0 6-8 12-8 12s-8-6-8-12a8 8 0 0 1 16 0Z"/>
                                            <circle cx="12" cy="10" r="3"/>
                                        </svg>
                                    </div>
                                    <div>
                                        <p class="fw-semibold mb-1">Dirección</p>
                                        <p class="text-muted mb-0">Av. Libertador 1234, Ciudad Capital</p>
                                        <p class="text-muted small mb-0">Código Postal: 1425</p>
                                    </div>
                                </div>
                                
                                <div class="d-flex align-items-start gap-3">
                                    <div class="icon-container">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                            <path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"/>
                                        </svg>
                                    </div>
                                    <div>
                                        <p class="fw-semibold mb-1">Teléfono</p>
                                        <p class="text-muted mb-0">+54 11 1234-5678</p>
                                        <p class="text-muted small mb-0">WhatsApp: +54 9 11 8765-4321</p>
                                    </div>
                                </div>
                                
                                <div class="d-flex align-items-start gap-3">
                                    <div class="icon-container">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                            <rect width="20" height="16" x="2" y="4" rx="2"/>
                                            <path d="m22 7-8.97 5.7a1.94 1.94 0 0 1-2.06 0L2 7"/>
                                        </svg>
                                    </div>
                                    <div>
                                        <p class="fw-semibold mb-1">Email</p>
                                        <p class="text-muted mb-0">info@institutosanmartin.edu</p>
                                        <p class="text-muted small mb-0">Admisiones: admisiones@institutosanmartin.edu</p>
                                    </div>
                                </div>
                                
                                <div class="d-flex align-items-start gap-3">
                                    <div class="icon-container">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                            <circle cx="12" cy="12" r="10"/>
                                            <polyline points="12 6 12 12 16 14"/>
                                        </svg>
                                    </div>
                                    <div>
                                        <p class="fw-semibold mb-1">Horario de Atención</p>
                                        <p class="text-muted mb-0">Lunes a Viernes: 8:00 - 18:00</p>
                                        <p class="text-muted small mb-0">Sábados: 9:00 - 13:00 (solo admisiones)</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="map-container">
                        <iframe 
                            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3283.849761425956!2d-58.38375908477024!3d-34.60373698045961!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x95bccacf8c4f63cf%3A0x8e8c6f7f6b5c8d8a!2sBuenos%20Aires%2C%20Argentina!5e0!3m2!1ses!2sus!4v1234567890123!5m2!1ses!2sus"
                            allowfullscreen
                            loading="lazy"
                            referrerpolicy="no-referrer-when-downgrade"
                            class="w-100 h-100">
                        </iframe>
                    </div>
                </div>
            </div>

            <div class="mt-5 p-4 bg-light rounded-3">
                <h3 class="text-center mb-4">Proceso de Admisión</h3>
                <div class="row g-4">
                    <div class="col-md-6 col-lg-3">
                        <h4>1. Solicitud</h4>
                        <p>Completa el formulario de contacto o agenda una cita informativa.</p>
                    </div>
                    <div class="col-md-6 col-lg-3">
                        <h4>2. Entrevista</h4>
                        <p>Entrevista con el equipo de admisiones y evaluación diagnóstica.</p>
                    </div>
                    <div class="col-md-6 col-lg-3">
                        <h4>3. Documentación</h4>
                        <p>Entrega de documentos requeridos y expedientes académicos.</p>
                    </div>
                    <div class="col-md-6 col-lg-3">
                        <h4>4. Matrícula</h4>
                        <p>Confirmación de cupo y proceso formal de matrícula.</p>
                    </div>
                </div>
                <div class="text-center mt-4">
                    <button class="btn btn-custom-primary" onclick="scrollToSection('contacto')">Iniciar Proceso de Admisión</button>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <div class="row g-4 mb-4">
                <div class="col-lg-3">
                    <div class="footer-brand">
                        <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                            <path d="M22 10v6M2 10l10-5 10 5-10 5z"/>
                            <path d="M6 12v5c3 3 9 3 12 0v-5"/>
                        </svg>
                        Instituto San Martín
                    </div>
                    <p class="text-white-50 mb-2">Formando líderes del mañana desde 1985 con excelencia académica y valores sólidos.</p>
                    <p class="small">
                        <a href="#" onclick="openModal('privacyPolicyModal')" class="text-primary-light text-decoration-underline cursor-pointer">Política de Privacidad</a>
                    </p>
                </div>

                <div class="col-lg-3">
                    <h3 class="text-white mb-3">Enlaces Rápidos</h3>
                    <ul class="footer-links">
                        <li><a href="#inicio">Inicio</a></li>
                        <li><a href="#nosotros">Nosotros</a></li>
                        <li><a href="#programas">Programas</a></li>
                        <li><a href="#instalaciones">Instalaciones</a></li>
                        <li><a href="#contacto">Contacto</a></li>
                    </ul>
                </div>

                <div class="col-lg-3">
                    <h3 class="text-white mb-3">Recursos</h3>
                    <ul class="footer-links">
                        <li><a href="#">Portal Estudiantil</a></li>
                        <li><a href="#">Calendario Académico</a></li>
                        <li><a href="#">Biblioteca Virtual</a></li>
                        <li><a href="#">Admisiones</a></li>
                        <li><a href="#">Becas y Ayudas</a></li>
                    </ul>
                </div>

                <div class="col-lg-3">
                    <h3 class="text-white mb-3">Síguenos</h3>
                    <p class="text-white-50 mb-3">Mantente al día con nuestras noticias y eventos.</p>
                    <div class="social-links">
                        <a href="#" class="social-link" aria-label="Facebook">
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                <path d="M18 2h-3a5 5 0 0 0-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 0 1 1-1h3z"/>
                            </svg>
                        </a>
                        <a href="#" class="social-link" aria-label="Instagram">
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                <rect width="20" height="20" x="2" y="2" rx="5" ry="5"/>
                                <path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"/>
                                <line x1="17.5" x2="17.51" y1="6.5" y2="6.5"/>
                            </svg>
                        </a>
                        <a href="#" class="social-link" aria-label="YouTube">
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                <path d="M22.54 6.42a2.78 2.78 0 0 0-1.94-2C18.88 4 12 4 12 4s-6.88 0-8.6.46a2.78 2.78 0 0 0-1.94 2A29 29 0 0 0 1 11.75a29 29 0 0 0 .46 5.33A2.78 2.78 0 0 0 3.4 19c1.72.46 8.6.46 8.6.46s6.88 0 8.6-.46a2.78 2.78 0 0 0 1.94-2 29 29 0 0 0 .46-5.25 29 29 0 0 0-.46-5.33z"/>
                                <polygon points="9.75 15.02 15.5 11.75 9.75 8.48 9.75 15.02"/>
                            </svg>
                        </a>
                        <a href="#" class="social-link" aria-label="LinkedIn">
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                <path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"/>
                                <rect width="4" height="12" x="2" y="9"/>
                                <circle cx="4" cy="4" r="2"/>
                            </svg>
                        </a>
                    </div>
                </div>
            </div>
            
            <div class="footer-bottom">
                <p>© 2024 Instituto San Martín. Todos los derechos reservados.</p>
                <p class="mt-2 small">
                    <a href="#" onclick="openModal('privacyPolicyModal')" class="text-white-50 text-decoration-none cursor-pointer">Política de Privacidad</a> | 
                    <a href="#" class="text-white-50 text-decoration-none">Términos y Condiciones</a> |
                    <a href="#" class="text-white-50 text-decoration-none">Mapa del Sitio</a>
                </p>
            </div>
        </div>
    </footer>

    <!-- Bootstrap JS Bundle with Popper -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js"></script>

    <script>
        // === FUNCIONES PRINCIPALES ===
        
        // Scroll suave a secciones
        function scrollToSection(id) {
            const element = document.getElementById(id);
            if (element) {
                element.scrollIntoView({
                    behavior: 'smooth',
                    block: 'start'
                });
            }
        }

        // Modales
        function openModal(id) {
            const modal = document.getElementById(id);
            if (modal) {
                modal.classList.add('active');
                document.body.style.overflow = 'hidden';
            }
        }

        function closeModal(id) {
            const modal = document.getElementById(id);
            if (modal) {
                modal.classList.remove('active');
                document.body.style.overflow = '';
            }
        }

        // Cerrar modal al hacer clic fuera
        document.addEventListener('click', (e) => {
            if (e.target.classList.contains('custom-modal')) {
                closeModal(e.target.id);
            }
        });

        // Cerrar modal con Escape
        document.addEventListener('keydown', (e) => {
            if (e.key === 'Escape') {
                const openModals = document.querySelectorAll('.custom-modal.active');
                openModals.forEach(modal => {
                    modal.classList.remove('active');
                });
                document.body.style.overflow = '';
            }
        });

        // Contador animado de estadísticas
        function animateCounters() {
            const counters = document.querySelectorAll('.stat-number');
            
            counters.forEach(counter => {
                const target = parseInt(counter.getAttribute('data-count'));
                const duration = 2000;
                const increment = target / (duration / 16);
                let current = 0;
                
                const updateCounter = () => {
                    current += increment;
                    if (current < target) {
                        counter.textContent = Math.floor(current);
                        requestAnimationFrame(updateCounter);
                    } else {
                        counter.textContent = target + (counter.getAttribute('data-count') === '98' ? '%' : '+');
                    }
                };
                
                const observer = new IntersectionObserver((entries) => {
                    if (entries[0].isIntersecting) {
                        updateCounter();
                        observer.unobserve(counter);
                    }
                });
                
                observer.observe(counter);
            });
        }

        // Manejo del formulario de contacto
        document.getElementById('contactForm')?.addEventListener('submit', function(e) {
            e.preventDefault();
            
            const name = document.getElementById('name').value.trim();
            const email = document.getElementById('email').value.trim();
            const message = document.getElementById('message').value.trim();
            
            if (!name || !email || !message) {
                alert('Por favor, complete todos los campos obligatorios');
                return;
            }
            
            if (!validateEmail(email)) {
                alert('Por favor, ingrese un email válido');
                return;
            }
            
            alert('¡Mensaje enviado correctamente! Nos pondremos en contacto contigo en breve.');
            this.reset();
        });

        // Validación de email
        function validateEmail(email) {
            const re = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
            return re.test(email);
        }

        // Efecto de scroll en navbar
        function handleScroll() {
            const navbar = document.getElementById('navbar');
            if (window.scrollY > 50) {
                navbar.classList.add('shadow');
                navbar.style.padding = '0.5rem 0';
            } else {
                navbar.classList.remove('shadow');
                navbar.style.padding = '';
            }
        }

        // Política de privacidad - Mostrar al cargar si no se ha aceptado
        function checkPrivacyPolicy() {
            if (!localStorage.getItem('privacyAccepted')) {
                setTimeout(() => {
                    openModal('privacyPolicyModal');
                }, 1000);
            }
        }

        // Manejo de aceptación de política de privacidad
        document.getElementById('acceptPrivacyBtn')?.addEventListener('click', () => {
            localStorage.setItem('privacyAccepted', 'true');
            closeModal('privacyPolicyModal');
            alert('Política de privacidad aceptada');
        });

        // === INICIALIZACIÓN ===
        document.addEventListener('DOMContentLoaded', () => {
            animateCounters();
            checkPrivacyPolicy();
            
            window.addEventListener('scroll', handleScroll);
            handleScroll();
        });
    </script>
</body>
</html>
