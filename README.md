# Simple-middleware

const middleware = function (req, res, next) {
  try{
    console.log(req.headers.api);
        let config = 'Api-key'
        res.status(200).send('xyz')
        if(config){
          return 'correct'
        }
        else{
          'wrong'
        }
        next()
  }
  catch(err){
    console.log(err.message);
  }
  }
