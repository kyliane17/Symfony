# lancement de l'application 
sudo service apache2 restart

# routes 

/**
 * @Route("/movie", name="app_movie")
 */

 # route exemple 
 
 http://172.27.174.107/html/SymfonyCine/public/movies/m

 # fonctions exemple 
 public function GetidMovie() : Response
    {
      return $this->render('movie/id.html.twig',['movieid'=>$this->_movies]);
    }

# mvc 
modèle view controller :  demnde du contolleur vers le modèle puis la vue 

# exemple de class et de namespace 
namespace App\Controller;

use Symfony\Bundle\FrameworkBundle\Controller\AbstractController;
use Symfony\Component\HttpFoundation\JsonResponse;
use Symfony\Component\HttpFoundation\Response;
use Symfony\Component\Routing\Annotation\Route;

class MovieController extends AbstractController

# controller 
controller ce trouve dans src -> controller 

# templates 
en .twig 
debut de block : {% block (nom du block) %}
fin de block : {% endblock %}